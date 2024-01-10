
1- Function Declaration:

FUNCTION palindrom(chaine:STRING) : BOOLEAN;

2- Variable Declarations:

VAR
    results :=BOOLEAN;
    sChaine :=STRING;
BEGIN

3- Palindrome Check:

    IF (chaine.lenth <=1) THEN 
        results := TRUE;

4- Recursive Check:     

       ELSE
        IF (chaine[0] = chaine[chaine.length-1]) THEN
            sChaine := Sous_chaine(chaine, 2, chaine.length-2); 
            palindrome(sChaine);

          
5- Result Assignment:            
            ELSE
            results:= FALSE
        END_IF
    END_IF

6- Return Statement:

    RETURN results;
END
