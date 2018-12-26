### CHAPTER 1
  1.1 Getting started 
    /* print "Hello world" in C */
  
    #include <stdio.h>                /* import standard input/output library. it is head file */
  
     main()                         /* a function named main */
     {                             /* statements of main */
         printf("Hello world\n"); /* function printf: output formatting function; \n represents the newline character*/
     }
     
   1.2 variable and arithmetic expressions     
   
      #include <stdio.h>

     main()
     {
          int fahr, celsius;
          int lower, upper, step;

           lower = 0;
           upper = 300;
           step = 20;

           fahr = lower;
           while (fahr <= upper) {
              celsius = 5 *(fahr - 32) / 9;
              printf("%d\t%d\n", fahr, celsius);
              fahr = fahr + step;
           }
    }

- comment 

      /* */
- declaration: all variables must be declared, it consists of a type name and a list of variables, 

      int fahr, celsius;
      int lower, upper, step;
- data types
  - char  character - a single byte
  - short short integer
  - long long integer
  - double double-prescision floating point
  - arrays
  - structures
  - unions
- right-justified

    printif("%3d %6d\n", fahr, celsius);   /* printed at least 3 and 6 characters wide */ 
    
    - %f     print as floating point
    - %6f    print as floating point at least 6 characters wide
    - %6.2f  print as floating point, at least 6 wide and 2 after decimal point
    - %o for octal, %x for hexadecimal, %c for character, %s for character string, %% for % itself
    
 - floating-point arithmetic instead of integer
 
   second version:
   
        #include <stdio.h>
        main()
        {
            float fahr, celsius;
            int lower, upper, step;

            lower = 0;
            upper = 300;
            step = 20;

            fahr = lower;
            while (fahr <= upper) {
                celsius = (5.0/9.0) *(fahr - 32.0);
                printf("%3.0f %6.1f\n", fahr, celsius);
                fahr = fahr + step;
             }
          }
          
 1.3 The for statement
 
        #include <stdio.h>
        main()
        {
            int fahr;

            for (fahr = 0; fahr<= 300; fahr = fahr + 20)
                printf("%3d %6.1f\n", fahr,(5.0/9.0)*(fahr-32));
         }
    
    1.4 Symbolic constants
          
          #define name replacement text
          
     second version
     
        #include <stdio.h>
        #define LOWER 0              /* Symbolic constant are written in upper case, no semicolon at the end, do not appear in declarations */
        #define UPPER 300
        #define STEP 20
        
        main()
        {
            int fahr;

            for (fahr = LOWER; fahr<= UPPER; fahr = fahr + STEP)
                printf("%3d %6.1f\n", fahr,(5.0/9.0)*(fahr-32));
         }
         
    1.5 Character input and output
    - getchar()     read the next input character
    - putchar()     print a character each time 
    
    
          
          
         
 
    
  
