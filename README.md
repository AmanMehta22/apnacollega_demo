#include<iostream>
using namespace std;
int main(){
    int pin=2080;
    int balance=10000;
    int a=1;
    while(a){
        int pin_check;
        cout<<"ENTER PIN : ";
        cin>>pin_check;
        if(pin==pin_check){
            int num;
            
            cout<<"------------------------PRESS 1 FOR WITHDRAW------------------------"<<endl;
            cout<<"------------------------PRESS 2 FOR BALANCE CHECK------------------------ "<<endl;
            cout<<"------------------------PRESS 3 FOR PIN GENERATION------------------------"<<endl;
            cout<<"------------------------PRESS 4 FOR STATEMENT------------------------"<<endl<<endl;
            cout<<"ENTER NUMBER : "<<endl;
            cin>>num;
            switch(num){
                case 1: 
                    cout<<"------------------------ENTER AMOUNT TO WITHDRAW : ------------------------"<<endl;
                    int withdraw;
                    cin>>withdraw;
                    if(withdraw<balance){
                        balance-=withdraw;
                        cout<<"------------------------"<<withdraw<<"/- SUCCESFULLY DEBITED------------------------ ";
                    }
                    else{
                        cout<<"------------------------INSUFFICIENT BALANCE------------------------ ";
                    }
                
                break;
                


                case 2:
                        cout<<"------------------------YOUR BALANCE IS "<<balance<<"/-------------------------";
                
                break;
                
                
                
                
                case 3:
                            cout<<"------------------------PRESS 1 FOR PIN UPDATION------------------------ "<<endl;
                            cout<<"------------------------PRESS 2 FOR NEW PIN GENERATION------------------------ "<<endl;
                            int num1;
                            cin>>num1;
                            int otp;
                            cout<<"------------------------ENTER OTP SENT ON YOUR MOBILE NUMBER VIA SMS------------------------ "<<endl;
                            cout<<"------------------------_____ON YOUR NUMBER xxxxxx9089_______________------------------------"<<endl;
                            cin>>otp;
                            if(100000<=otp<=999999){

                                switch(num1){

                                    case 1:
                                        int pin_update;
                                        cout<<"------------------------ENTER NEW PIN :------------------------"<<endl;
                                        cin>>pin_update;
                                        pin=pin_update;
                                        cout<<"------------------------PIN UPDATED SUCCESSFULLY------------------------ "<<endl;
                                    break;

                                    case 2:

                                        int pin_generation;
                                        cout<<"------------------------ENTER NEW PIN :------------------------"<<endl;
                                        cin>>pin_generation;
                                        pin=pin_generation;
                                        cout<<"------------------------PIN GENERATED SUCCESSFULLY------------------------"<<endl;
                                    

                                }

                            }
                            else{
                                        cout<<"------------------------INVALID OTP !------------------------"<<endl;
                                }
                break;

                case 4:

                            cout<<endl;
                            cout<<"11/11/2024  10:24  7033"<<endl;
                            cout<<"-------------------"<<endl;
                            cout<<"xxxxxxxxxxxx2355"<<endl;
                            cout<<"AXIS BANK"<<endl;
                            cout<<"HINOO BRANCH"<<endl;
                            cout<<"TERMINAL IC 70135"<<endl;
                            cout<<"11/11/2024  123564"<<endl;
                            cout<<endl;
                            cout<<"-------------------"<<endl;
                            cout<<"MINI STATEMENT CHECKING"<<endl;
                            cout<<"ACCOUNT xxxxxxxxxxxx2355"<<endl;
                            cout<<""<<endl;
                            cout<<"-------------------"<<endl;
                            cout<<"NOV02 ATM W/D           5045.28"<<endl;
                            cout<<"NOVO4 ATM C/D           8000.00"<<endl;
                            cout<<"NOV08 DEPOSIT            800.00"<<endl;
                            cout<<"NOV10 POS RETURN         100.20"<<endl;
                            cout<<"-------------------"<<endl;
                            cout<<"LEDGER BAL $           "<<balance<<endl;
                            break;
            }
        }

        else{
                            cout<<"------------------------INVALID PIN !------------------------"<<endl;
            }
                cout<<endl;
                cout<<"DO YOU WANT TO DO FURTHER ?(1 FOR YES / 0 FOR NO ) :";
                cin>>a;
    }
}
