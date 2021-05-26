# cs50-labs-2021-x-population #include<cs50.h>
#include<Stdio.h>

  main()
  {
     int i,j,n,count,y,coco;
    printf("enter the starting population");

     scanf("%d",&n);
     coco=1;

      if(n<9)
      {
          do{

            printf("no dumb ass enter again\n");
            scanf("%d",&n);
     coco++;
           if(coco>10)
             {


            printf("seriously dont be a dumb ass population cannot be lesser than 9\n");

             }

          }while(n<9);


      }



    printf("starting population = %d\n",n);

    printf("enter the ending population");
    scanf("%d",&j);

      if(j<n)
      {
          do{
            printf("enter the ending population again ,idiot");
            scanf("%d",&j);



          }while(j<n);




      }

    printf("ending population %d\n",j);

     n=n+(n/3)-(n/4);

     count=1;

     if(n<j)
     {
       do
       {
            n=n+(n/3)-(n/4);

             count++;

       }while(n<j);



     }
     printf(" years would be=%i\t\n",count);






    }
