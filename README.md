# C++ Bank-Application-Project
These is the Banking Application that's helps you to managed the all customer account details and transactions, loans enquiry etc.👍😎

#include<iostream>
#include<windows.h>

using namespace std;

class Bank
{
   private:
   string userName,uNam,fname,mname,lname,addr,city,branch,date,ph,paswrd,pass,acc="6788932156";
   int pin,bal,type;

   public:
   int depBal,withBal;

   void setnewAcc()
   {
       cout<<endl;
       cout<<"\t~~~~~~~~~~~~~~~~~~~~~~~~"<<endl;
       cout<<"\t| NEW ACCOUNT OPENING |"<<endl;
       cout<<"\t~~~~~~~~~~~~~~~~~~~~~~~~"<<endl;
       cout<<endl;
       y:
       cout<<"   ----------------------------------"<<endl;
       cout<<"   | 1]  SAVING ACCOUNT             |"<<endl;
       cout<<"   | 2]  CURRENT ACCOUNT            |"<<endl;
       cout<<"   ----------------------------------"<<endl;
       cout<<endl;
       cout<<"SELECT ACCOUNT TYPE : ";
       cin>>type;
       if(type==1)
       {
            cout<<endl;
            cout<<"\t~~~~~~~~~~~~~~~~~~~"<<endl;
            cout<<"\t| SAVING ACCOUNT |"<<endl;
            cout<<"\t~~~~~~~~~~~~~~~~~~~"<<endl;
            cout<<endl;
            cout<<"ENTER YOUR FIRST NAME  : ";
            cin>>fname;
            cout<<endl;
            cout<<"ENTER YOUR MIDDLE NAME : ";
            cin>>mname;
            cout<<endl;
            cout<<"ENTER YOUR LAST NAME   : ";
            cin>>lname;
            cout<<endl;
            cout<<"ENTER PHONE NO         : ";
            cin>>ph;
            cout<<endl;
            cout<<"ENTER YOUR ADDRESS     : ";
            cin>>addr;
            cout<<endl;
            cout<<"ENTER CITY             : ";
            cin>>city;
            cout<<endl;
            cout<<"ENTER PIN CODE         : ";
            cin>>pin;
            cout<<endl;
            cout<<"ENTER BRANCH NAME      : ";
            cin>>branch;
            cout<<endl;
            cout<<"ENTER ACCOUNT OPENING BALANCE   : ";
            cin>>bal;
            cout<<endl;
            cout<<"ENTER DATE             : ";
            cin>>date;
            cout<<endl;
            cout<<"CREAT USERNAME         : ";
            cin>>userName;
            cout<<endl;
            cout<<"CREAT PASSWORD         : ";
            cin>>paswrd;
            cout<<endl;
            system("cls");
            loader();
            system("cls");
       }
       else if(type==2)
       {
            cout<<endl;
            cout<<"\t~~~~~~~~~~~~~~~~~~~~~"<<endl;
            cout<<"\t| CURRENT ACCOUNT |"<<endl;
            cout<<"\t~~~~~~~~~~~~~~~~~~~~~"<<endl;
            cout<<endl;
            cout<<"ENTER YOUR FIRST NAME  : ";
            cin>>fname;
            cout<<endl;
            cout<<"ENTER YOUR MIDDLE NAME : ";
            cin>>mname;
            cout<<endl;
            cout<<"ENTER YOUR LAST NAME   : ";
            cin>>lname;
            cout<<endl;
            cout<<"ENTER PHONE NO         : ";
            cin>>ph;
            cout<<endl;
            cout<<"ENTER YOUR ADDRESS     : ";
            cin>>addr;
            cout<<endl;
            cout<<"ENTER CITY             : ";
            cin>>city;
            cout<<endl;
            cout<<"ENTER PIN CODE         : ";
            cin>>pin;
            cout<<endl;
            cout<<"ENTER BRANCH NAME      : ";
            cin>>branch;
            cout<<endl;
            cout<<"ENTER ACCOUNT OPENING BALANCE   : ";
            cin>>bal;
            cout<<endl;
            cout<<"ENTER DATE             : ";
            cin>>date;
            cout<<endl;
            cout<<"CREAT USERNAME         : ";
            cin>>userName;
            cout<<endl;
            cout<<"CREAT PASSWORD         : ";
            cin>>paswrd;
            cout<<endl;
            system("cls");
            loader();
            system("cls");
       }
       else
       {
           cout<<endl;
           cout<<"INVALID INPUT,PLEASE SELECT FROM ABOVE..!"<<endl;
           cout<<endl;
           goto y;
       }
   }
   void getnewAcc()
   {
       system("cls");
       loader();
        system("cls");
        cout<<endl;
        cout<<"\t~~~~~~~~~~~~~~~~~~~~~~~~~~"<<endl;
        cout<<"\t| ACCOUNT HOLDER DETAILS |"<<endl;
        cout<<"\t~~~~~~~~~~~~~~~~~~~~~~~~~~"<<endl;
        cout<<endl;
        cout<<"----------------------------------------"<<endl;
        cout<<"~~~~~~~~~~~~~*::|CLERCK |::*~~~~~~~~~~~~~"<<endl;
        cout<<endl;
        cout<<"ACCOUNT HOLDER : "<<fname<<" "<<mname<<" "<<lname<<endl;
        cout<<endl;
        cout<<"PHONE NO       : "<<ph<<endl;
        cout<<endl;
        cout<<"ADDRESS        : "<<addr<<endl;
        cout<<endl;
        cout<<"CITY           : "<<city<<endl;
        cout<<endl;
        cout<<"PIN CODE       : "<<pin<<endl;
        cout<<endl;
        cout<<"BRANCH         : "<<branch<<endl;
        cout<<endl;
        cout<<"DATE           : "<<date<<endl;
        cout<<endl;
        cout<<"----------------------------------------"<<endl;
        cout<<"~~~~~~~~~~~~~~~~~~~~**~~~~~~~~~~~~~~~~~~~~"<<endl;
   }
   void cusLogin()
   {

       cout<<endl;
       cout<<"\t~~~~~~~~~~~~~~~~~~~~~~~"<<endl;
       cout<<"\t| USER/CUSTOMER LOGIN |"<<endl;
       cout<<"\t~~~~~~~~~~~~~~~~~~~~~~~"<<endl;
       cout<<endl;
       z:
       cout<<endl;
       cout<<"ENTER USERNAME : ";
       cin>>uNam;
       cout<<endl;
       cout<<"ENTER PASSWORD : ";
       cin>>pass;
       system("cls");
       loader();
        system("cls");
       cout<<endl;
       if(uNam==userName && pass==paswrd)
       {
            cout<<"USERNAME OR PASSWORD MATCH SUCCESFULLY....."<<endl;
            cout<<endl;
            cout<<"----------------------------------------"<<endl;
            cout<<endl;
            cout<<"ACCOUNT HOLDER : "<<fname<<" "<<mname<<" "<<lname<<endl;
            cout<<endl;
            cout<<"ACCOUNT NUMBER : "<<acc<<endl;
            cout<<endl;
            cout<<"BALANCE        : "<<bal<<" Rs/-"<<endl;
            cout<<endl;
            cout<<"PHONE NO       : "<<ph<<endl;
            cout<<endl;
            cout<<"ADDRESS        : "<<addr<<endl;
            cout<<endl;
            cout<<"CITY           : "<<city<<endl;
            cout<<endl;
            cout<<"PIN CODE       : "<<pin<<endl;
            cout<<endl;
            cout<<"BRANCH         : "<<branch<<endl;
            cout<<endl;
            cout<<"DATE           : "<<date<<endl;
            cout<<endl;
            cout<<"----------------------------------------"<<endl;
        }
       else
       {
           cout<<"INCORRECT USERNAME OR PASSWORD, TRY AGAIN..!"<<endl;

           goto z;
       }
   }
   void balEnq()
   {
       int enqType;
       cout<<endl;
       cout<<"\t~~~~~~~~~~~~~~~~~~~"<<endl;
       cout<<"\t| BALANCE ENQUIRY |"<<endl;
       cout<<"\t~~~~~~~~~~~~~~~~~~~"<<endl;
       cout<<endl;
       c:
       cout<<"   --------------------------------"<<endl;
       cout<<"  | 1] BALANCE DEDUCTION QUIRY |"<<endl;
       cout<<"  | 2] CHECK ACCOUNT BALANCE   |"<<endl;
       cout<<"   --------------------------------"<<endl;
       cout<<endl;
       cout<<"SELECT ENQUIRY TYPE : ";
       cin>>enqType;
       system("cls");
       loader();
        system("cls");
       if(enqType==1)
       {
           cout<<endl;
           cout<<"\t~~~~~~~~~~~~~~~~"<<endl;
           cout<<"\t|DEDUCTION QUIRY |"<<endl;
           cout<<"\t~~~~~~~~~~~~~~~~"<<endl;
           cout<<endl;
           cout<<"---------------------------------------------------------------------------------"<<endl;
           cout<<"NOTE 1 :- ACCOUNT CASH LIMIT 500 Rs/-"<<endl;
           cout<<"NOTE 2 :- WHEN LESS THAN 500 Rs/- DEDUCTED 18.00 Rs/- MONTHLY"<<endl;
           cout<<"NOTE 3 :- DEDUCTED 177 Rs/- WHEN YOU WILL NOT USE ATM IN 3 MONTHS OF DURATION"<<endl;
           cout<<"---------------------------------------------------------------------------------"<<endl;
       }
       else if(enqType==2)
       {
           cout<<endl;
           cout<<"\t~~~~~~~~~~~~~~~~"<<endl;
           cout<<"\t|CHECK BALANCE |"<<endl;
           cout<<"\t~~~~~~~~~~~~~~~~"<<endl;
           cout<<endl;
           m:
           cout<<endl;
           cout<<"ENTER USERNAME : ";
           cin>>uNam;
           cout<<endl;
           cout<<"ENTER PASSWORD : ";
           cin>>pass;
           system("cls");
            loader();
            system("cls");
           cout<<endl;
           if(uNam==userName && pass==paswrd)
           {
                 cout<<"USERNAME OR PASSWORD MATCH SUCCESFULLY....."<<endl;
                 cout<<endl;
                 cout<<"----------------------------------------"<<endl;
                 cout<<"ACCOUNT HOLDER : "<<fname<<" "<<mname<<" "<<lname<<endl;
                 cout<<endl;
                 cout<<"ACCOUNT NUMBER : "<<acc<<endl;
                 cout<<endl;
                 cout<<"ACCOUNT BALANCE : "<<bal<<" Rs/-"<<endl;
                 cout<<"----------------------------------------"<<endl;
           }
          else
           {
               cout<<endl;
               cout<<"INCORRECT,USERNAME OR PASSWORD,TRY AGAIN...!"<<endl;
               cout<<endl;
               goto m;
           }
       }
       else
       {
           cout<<endl;
           cout<<"INVALID INPUT,PLEASE SELECT FROM ABOVE..!"<<endl;
           cout<<endl;
           goto c;
       }
   }
   void tranSact()
   {
       int traType,depBal,withBal;
        cout<<endl;
        cout<<"\t~~~~~~~~~~~~~~~~"<<endl;
        cout<<"\t| TRANSACTIONS |"<<endl;
        cout<<"\t~~~~~~~~~~~~~~~~"<<endl;
        cout<<endl;
        k:
        cout<<endl;
        cout<<"ENTER USERNAME : ";
        cin>>uNam;
        cout<<endl;
        cout<<"ENTER PASSWORD : ";
        cin>>pass;
        system("cls");
       loader();
        system("cls");
        cout<<endl;
        if(uNam==userName && pass==paswrd)
        {
            cout<<"USERNAME OR PASSWORD MATCH SUCCESFULLY....."<<endl;
            cout<<endl;
            a:
            cout<<"   ----------------------"<<endl;
            cout<<"   | 1]  DEPOSITE CASH  |"<<endl;
            cout<<"   | 2]  WITHDRAW CASH  |"<<endl;
            cout<<"   ----------------------"<<endl;
            cout<<endl;
            cout<<"SELECT TRANSCACTION TYPE : ";
            cin>>traType;
            system("cls");
             loader();
            system("cls");
            cout<<endl;
            if(traType==1)
            {
                cout<<"ENTER CASH TO DEPOSITE : ";
                cin>>depBal;
                cout<<endl;
                loader();
                system("cls");
                bal=bal+depBal;
                cout<<endl;
                cout<<"~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~"<<endl;
                cout<<endl;
                cout<<"CASH DEPOSITED SUCESSFULLY IN YOUR ACCOUNT"<<endl;
                cout<<endl;
                cout<<"YOUR ACCOUNT BALANCE : "<<bal<<" Rs/-"<<endl;
                cout<<endl;
                cout<<"THANK YOU!,FOR TRANSACTION.."<<endl;
                cout<<endl;
                cout<<"~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~"<<endl;
            }
            else if(traType==2)
            {
                cout<<endl;
                cout<<"ENTER CASH TO WITHDRAW : ";
                cin>>withBal;
                cout<<endl;
                loader();
                system("cls");
                if(bal>=withBal)
                {
                    bal=bal-withBal;
                }
                cout<<endl;
                cout<<"~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~"<<endl;
                cout<<endl;
                cout<<"CASH DEBITED SUCESSFULLY FROM YOUR ACCOUNT"<<endl;
                cout<<endl;
                cout<<"YOUR ACCOUNT BALANCE : "<<bal<<" Rs/-"<<endl;
                cout<<endl;
                cout<<"THANK YOU!,FOR TRANSACTION.."<<endl;
                cout<<endl;
                cout<<"~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~"<<endl;
            }
            else
            {
                       cout<<endl;
                       cout<<"INVALID INPUT,PLEASE SELECT FROM ABOVE..!"<<endl;
                       cout<<endl;
                       goto a;
            }
        }
        else
        {
             cout<<endl;
             cout<<"INCORRECT,USERNAME OR PASSWORD,TRY AGAIN...!"<<endl;
             cout<<endl;
             goto k;
        }
   }
   void manager()
   {
            cout<<"~~~~~~~~~~~~~*::|MANAGER |::*~~~~~~~~~~~~~"<<endl;
            cout<<endl;
            cout<<"ACCOUNT NUMBER : "<<acc<<endl;
            cout<<endl;
            cout<<"BALANCE        : "<<bal<<" Rs/-"<<endl;
            cout<<endl;
            loanEnq();
            cout<<"~~~~~~~~~~~~~~~~~~~~**~~~~~~~~~~~~~~~~~~~~"<<endl;
   }
   private:
   void loanEnq()
   {
       int pre,lpre,lamt,irt,yrs,tamt,mamt;
       string ltype;
        cout<<endl;
        cout<<"\t~~~~~~~~~~~~~~~~~"<<endl;
        cout<<"\t| LOANS/ENQUIRY |"<<endl;
        cout<<"\t~~~~~~~~~~~~~~~~~"<<endl;
        cout<<endl;
        n:
        cout<<"      ----------------------"<<endl;
        cout<<"      | 1]  LOAN ENQUIRY   |"<<endl;
        cout<<"      | 2]  TAKE LOAN      |"<<endl;
        cout<<"      ----------------------"<<endl;
        cout<<endl;
        cout<<"SELECT YOUR PREFERNCE : ";
        cin>>pre;
        system("cls");
        loader();
        system("cls");
        cout<<endl;
        if(pre==1)
        {
            x:
              cout<<"\t~~~~~~~~~~~~~~~~~~~~~~~~~~~~~"<<endl;
              cout<<"\t|  ***::TYPES OF LOANS::*** |"<<endl;
              cout<<"\t~~~~~~~~~~~~~~~~~~~~~~~~~~~~~"<<endl;
              cout<<"\t|  -: LOANS/RATE OF INTR :- |"<<endl;
              cout<<"\t|                           |"<<endl;
              cout<<"\t| 1) PERSONAL LOAN   : 11%  |"<<endl;
              cout<<"\t| 2) HOME LOAN       : 8%   |"<<endl;
              cout<<"\t| 3) EDUCATION LOAN  : 9%   |"<<endl;
              cout<<"\t| 4) GOLD LOAN       : 7%   |"<<endl;
              cout<<"\t|                           |"<<endl;
              cout<<"\t-----------------------------"<<endl;
              cout<<endl;
              cout<<"SELECT LOAN PREFERENCE : ";
              cin>>lpre;
              system("cls");
              loader();
              system("cls");
              cout<<endl;
              if(lpre==1)
              {
                  cout<<"YOU HAVE SELECT PERSONAL LOAN..!"<<endl;
                  cout<<endl;
                  cout<<"------------------------------------------------------------------------------"<<endl;
                  cout<<"NOTE 1 : EMI STARTING FROM 1878 Rs/- per Lac MONTHLY FOR 5 YEARS"<<endl;
                  cout<<"NOTE 2 : YOU ARE ELIGIBLE FOR TAKING LOAN WHEN AGE RANGES FROM 21 TO 60 YEARS"<<endl;
                  cout<<"------------------------------------------------------------------------------"<<endl;
              }
              else if(lpre==2)
              {
                  cout<<"YOU HAVE SELECT HOME LOAN..!"<<endl;
                  cout<<endl;
                  cout<<"------------------------------------------------------------------------------"<<endl;
                  cout<<"NOTE 1 : EMI STARTING FROM 741 Rs/- per Lac MONTHLY FOR 30 YEARS"<<endl;
                  cout<<"NOTE 2 : YOU ARE ELIGIBLE FOR TAKING LOAN WHEN AGE RANGES FROM 21 TO 60 YEARS"<<endl;
                  cout<<"------------------------------------------------------------------------------"<<endl;
              }
              else if(lpre==3)
              {
                  cout<<"YOU HAVE SELECT EDUCATION LOAN..!"<<endl;
                  cout<<endl;
                  cout<<"-------------------------------------------------------------------------------------"<<endl;
                  cout<<"NOTE 1 : EMI STARTING FROM 11870 Rs/- per Lac MONTHLY OF LOAN AMT 10 Lac FOR 15 YEARS"<<endl;
                  cout<<"NOTE 2 : YOU ARE ELIGIBLE FOR TAKING LOAN WHEN AGE RANGES FROM 16 TO 35 YEARS"<<endl;
                  cout<<"-------------------------------------------------------------------------------------"<<endl;
              }
              else if(lpre==4)
              {
                  cout<<"YOU HAVE SELECT GOLD LOAN..!"<<endl;
                  cout<<endl;
                  cout<<"------------------------------------------------------------------------------"<<endl;
                  cout<<"NOTE 1 : EMI STARTING FROM 741 Rs/- per Lac MONTHLY FOR 5 YEARS"<<endl;
                  cout<<"NOTE 2 : YOU ARE ELIGIBLE FOR TAKING LOAN WHEN AGE RANGES FROM 25 TO 60 YEARS"<<endl;
                  cout<<"------------------------------------------------------------------------------"<<endl;
              }
              else
              {
                    cout<<endl;
                    cout<<"INVALID INPUT,PLEASE SELECT FROM ABOVE..!"<<endl;
                    cout<<endl;
                    goto x;
              }
        }
        else if(pre==2)
        {
                  cout<<"\t~~~~~~~~~~~~~~~~~~~~~~~~~~~~~"<<endl;
                  cout<<"\t|  ***::TYPES OF LOANS::*** |"<<endl;
                  cout<<"\t~~~~~~~~~~~~~~~~~~~~~~~~~~~~~"<<endl;
                  cout<<"\t|  -: LOANS/RATE OF INTR :- |"<<endl;
                  cout<<"\t|                           |"<<endl;
                  cout<<"\t| 1) PERSONAL LOAN   : 11%  |"<<endl;
                  cout<<"\t| 2) HOME LOAN       : 8%   |"<<endl;
                  cout<<"\t| 3) EDUCATION LOAN  : 9%   |"<<endl;
                  cout<<"\t| 4) GOLD LOAN       : 7%   |"<<endl;
                  cout<<"\t|                           |"<<endl;
                  cout<<"\t-----------------------------"<<endl;
                  cout<<endl;
                  cout<<"ENTER LOAN TYPE       : ";
                  cin>>ltype;
                  cout<<endl;
                  cout<<"ENTER LOAN AMOUNT     : ";
                  cin>>lamt;
                  cout<<endl;
                  cout<<"ENTER INTEREST RATE   : ";
                  cin>>irt;
                  cout<<endl;
                  cout<<"ENTER NUMBER OF YEARS : ";
                  cin>>yrs;
                  system("cls");
                  loader();
                  system("cls");
                  cout<<endl;
                  cout<<"~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~"<<endl;
                  tamt=lamt+((yrs*lamt*irt)/100.00);
                  mamt=tamt/(yrs*12);
                  cout<<endl;
                  cout<<"LOAN                      : "<<ltype<<endl;
                  cout<<endl;
                  cout<<"TOTAL AMOUNT TO BE PAID   : "<<tamt<<" Rs/-"<<endl;
                  cout<<endl;
                  cout<<"TOTAL INTEREST            : "<<tamt-lamt<<" Rs/-"<<endl;
                  cout<<endl;
                  cout<<"MONTHLY AMOUNT TO BE PAID : "<<mamt<<" Rs/-"<<endl;
                  cout<<endl;
                  cout<<"~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~"<<endl;
        }
        else
        {
              cout<<endl;
              cout<<"INVALID INPUT,PLEASE SELECT FROM ABOVE..!"<<endl;
              cout<<endl;
              goto n;
        }
   }
   void loader()
   {
         int bar1=177,bar2=219;

                cout<<"\n\n\n\t\t\t\tWAIT A MINUTE.....";
                cout<<"\n\n\n\t\t\t\t";
                for(int i=0;i<25;i++)
                cout<<(char)bar1;

                cout<<"\r";
                cout<<"\t\t\t\t";
                for(int i=0;i<25;i++)
                {
                    cout<<(char)bar2;
                    Sleep(80);
                }
   }
};

int main()
{
    system("COLOR 0E");
    int n,i,choice;
    i=1;
    Bank c1,c2;
    cout<<"\n\t\xB3\xB2=\xB2=\xB2-\xB3 HDFC BANK SYSTEM \xB3\xB2=\xB2=\xB2-\xB3\n\n"<<endl;

    while(i)
    {
      if(choice!=0)
      {
            cout<<endl;
            cout<<"     ----------------------------------------"<<endl;
            cout<<"     --^--^--^--^--^-::MENU::-^--^--^--^--^--"<<endl;
            cout<<"     | 1] NEW ACCOUNT                       |"<<endl;
            cout<<"     | 2] USER/CUSTOMER LOGIN               |"<<endl;
            cout<<"     | 3] ACCOUNT HOLDER DETAILS            |"<<endl;
            cout<<"     | 4] BALANCE ENQUIRY                   |"<<endl;
            cout<<"     | 5] TRANSACTIONS                      |"<<endl;
            cout<<"     | 6] LOANS/ENQUIRY                     |"<<endl;
            cout<<"     | 0] EXIT/CLEAR                        |"<<endl;
            cout<<"     |                                      |"<<endl;
            cout<<"     ----------------------------------------"<<endl;
            cout<<endl;
      }
      cout<<"SELECT FROM MENU : ";
      cin>>choice;
      system("cls");
      cout<<endl;
      int bar1=177,bar2=219;

    cout<<"\n\n\n\t\t\t\tWAIT A MINUTE.....";
    cout<<"\n\n\n\t\t\t\t";
    for(int i=0;i<25;i++)
    cout<<(char)bar1;

    cout<<"\r";
    cout<<"\t\t\t\t";
    for(int i=0;i<25;i++)
    {
        cout<<(char)bar2;
        Sleep(50);
    }
    system("cls");
    cout<<endl;

        switch(choice)
        {
            case 1:
            c1.setnewAcc();
            break;

            case 2:
            c1.cusLogin();
            break;

            case 3:
            c1.getnewAcc();
            break;

            case 4:
            c1.balEnq();
            break;

            case 5:
            c1.tranSact();
            break;

            case 6:
            c1.manager();
            break;

            case 0:
            cout<<"EXIT/CLEAR"<<endl;
            cout<<"~~~~~~~~~~~~~~~~~~~~~~~~:: THANK YOU FOR USING OUR BANKING APPLICATION ::~~~~~~~~~~~~~~~~~~~~~~~~"<<endl;
            i=0;
            break;
        }
    }
    return 0;
}

