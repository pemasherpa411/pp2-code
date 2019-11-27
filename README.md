#include <iostream>
#include <cstdlib>
#include <string>

using namespace std;



int main()

{



// area decision variables

int areaChoice1, direction;

string armory, evidence;


// stat variables

int str = 10, luck = 10, intel = 10, agil = 10, hp = 25;


// enemy variables

int z1HP = 5;

string attChoice, attChoice2;



cout << "\t\t\t*__________________________*\n"

     << "\t\t\t   Welcome to Mission Cops \n"

     << "\t\t\t*__________________________*\n\n\n\n"



     << "You've watch enough zombie shows but you never thought it would be a reality, and now it's complete chaos. You and your partner aim for the heads of a hoard of zombie and fire off a few more rounds while you let in some uninfected off the street. You both slam the doors shut.";


     do{

cout<< " What would you like to do?\n\n"

            << "1 - Armory\n"

            << "2 - Evidence room\n"

            << "3 - Check on survivors\n"

            << "4 - Watch news\n"

            << "5 - I need to find my wife!\n\n"



            << "Enter number choice: \n\n";

        cin >>areaChoice1;

        cout << "\n";



    switch (areaChoice1){

        case 1:

               cout << "You enter the armory to and first notice is the AR rifles. Tasers won't do any good anymore.\n\n"



                    << "Would you like to pickup an AR rifle?\n"

                    << "Enter 'yes' or 'no': \n\n";

                    cin >> armory;

                    cout << "\n";

                    if (armory == "yes")

                    {

                    intel += 2;

                       cout <<"Can't go wrong with more firepower. You sling the rifle across your chest and grab a few mags.\n\n"

                            <<"Your intelligence has increased and is now " << intel << "\n\n";

                    }

                    else

                    {

                       cout << "I'll stick to the glock.\n\n";

                       }

               break;

        case 2:

               cout << "You enter the evidence room where everything is in plastic bags, and you have memories of crimes you've solved. You notice there's a live grenade mixed into the evidence.\n\n"


                    << "Would you like to pickup the grenade?\n"

                    << "Enter 'yes' or 'no': \n\n";

            cin >> evidence;

            cout << "\n";

            if (evidence == "yes")

            {

            luck += 2;

               cout <<"No better time to have something that goes boom. You pick up the grenade, notice it's weight, and place it on your cargo pocket.\n"

                    <<"Your luck has increased and is now " << luck << "\n\n";

            }

            else

            {

               cout << "It's a bit excessive and the shrapnel could hit innocent lives.\n\n";

               }

               break;

        case 3:

               str += 5;

               luck += 5;

               intel += 5;

               agil += 5;



               cout << "Entering the waiting room you see survivors who are completley distraught. Your partner in crime hands you a coffee. Now that you've had your coffee, your stats will increase\n\n"

                    << "Your stats are now: \n\n"

                    << str << " Strength\n"

                    << luck << " Luck\n"

                    << intel << " Intelligence\n"

                    << agil << " Agility\n\n";



               break;

        case 4:

               cout << "The news is reporting that the phone lines are down and telling everyone to go to the nearest police stations to stay safe. You think that's good idea; there's plenty of firepower in the armory to keep people safe.\n\n";

               break;

       case 5:

               cout << "All of a sudden you remember your wife is in all this mess and wonder if she's safe. It time to go look for her at the hospital.\n\n";

        default:

               cout << "Invalid entry.\n";

        }

    }while (areaChoice1 !=5);



               cout << "As you gather your things and run out to the back door to the parking lot, you get your gun ready. Others have been leaving the station without telling anyone to get their families too? Theirs a zombie that come up from behind you, but the parking lot is fenced in, so you dont know how it got in. Would you like to Run or Attack?\n\n"

                    << "Enter 'run' or 'attack'\n\n";

               cout << "Zombie HP: " << z1HP << "     Your HP: " << hp << "\n\n";



                    cin >> attChoice;



                    if (attChoice == "run")

                    {

                       if (agil > 12)

                          {

                               cout << "All that exercise paid off and you run like the wind to your police car in record time.";

                          }

                       else

                          {

                               cout << "As your starting to run, you trip on your self.";

                          }

                    }

                    else

                        {

                          cout << "\t\t\t*__________________________*\n"

                               << "\t\t\t      Zombie Attack     \n"

                               << "\t\t\t*__________________________*\n\n\n"



                               << "\nYou shoot the zombie & do 3 damage\n\n";

                          z1HP -= 3;

                          cout << "Zombie horde HP: " << z1HP << "\n\n";

                          cout << "The zombie now attacks you and does 5 damage\n\n";

                          hp -= 5;

                          cout << "Your HP: " << hp << "\n\n";

                          cout << "You shoot the zombie and do 3 damage\n\n";

                          z1HP -= 3;

                          cout << "Zombie horde HP: " << z1HP << "\n\n"



                               << "After a hard fight, you defeat your undead enemy. This \n"

                               << "attack caused some damage and you now have " << hp << " HP.\n\n";





                               do{

                          cout << "Now that you're safe inside your police car, you need to decide where you would like to go first:\n\n"

                               << "1 - Gas Station\n"

                               << "2 - House\n"

                               << "3 - Mall\n"

                               << "4 - Hospital\n"

                               << "Enter number choice: \n\n";



                      cin  >> direction;


                                switch (direction){

                                   case 1: cout << "You decide to get some gas.\n\n";


                                           break;



                                   case 2: cout << "You decide to check the house.\n";

                                           break;



                                   case 3: cout << "She might be at the mall.\n\n";

                                           break;

                                   case 4: cout << "You decide to go to the hospital where she works as a nurse.\n\n";

                                           break;



                                           default:

                                           cout << "Invalid entry.\n\n";

                                           break;






               //player finding is wife in the mall

//mall   //mall  //mall
cout << " You are now in the mall."
 << "you might find your wife here else go to hospital. I'm sure you'll find there if not here.\n"
 switch (Mallchoice)
 {
 case 1:
     cout <<end<< "Here you're are in the mall.\n\n";
     cout << "Do you wanna check if someone here?";
     if (key=="yes")
        cout <<"You're entered now in the mall.\n"
            <<" You will have to check all over the mall in order to find your wife.\n";
 }
     else{
        cout <<"You will sure find in the Hospital.\n";
     }
     break;
     case 2:
    cout<< "We have three section in the mall."
        <<"where you wanna search her";
        cout<< "1 - Reception\n"
            <<"2- clothing section\n"
            <<"3- security area\n"
        cin>> mallchoice;
        cout<<"\n";

        switch (Receptionchoice)
     {
     case 1:
        if (key=="yes")
            cout<< " there is no one here. Go to check in the Clothing section or security area.\n";

     }
     else{
            cout<< "You can check in Clothing section or security area.\n";

     }
     break;
     switch (Clothingsectionchoice)
     {
       case 2:
           cout<< "You might find here else you can go to clothing section\n ";
     }
      else{
      cout<< "you can find in the Security area\n"
    }
break;
cin>>attChoice2;
if (attChoice2== "run")
    cout<<" Zombies are coming towards you. Get out as soon as possible"
    cout<<" zombies attacking"
    cout<<"\t\t\t*__________________________*\n";
else {
          cout<< "you're alive and still have a hope to find your wife"; //gets out of the mall
     }
         else {
              cout << "You have died. and No more chance to find your wife" <<endl;

        }
        break;
        // now you're out of the mall and heading towards the hospital.
        cout<<"I'm 100% she is there.\n"

    }while (direction != 1 & direction !=3) ;


// Hospital             // Hospital                     // Hospital
cout <<"You have now reached the hospital and parked your car outside the entrance."
    << " This is the last place where your wife should be.\n"
    << "You close your eyes, take a deep breath, and walk inside...\n"
    << "Enter any key to continue...";
    cin >> continue2;

    cout <<"\n\nIt is quiet here and the emergency lights are on.\n";
    do{
    cout <<"\nWhere would you like to search?\n";
cout<< "1 - Surgery Room\n"
	<< "2 - Reception\n"
	<< "3 - Bathroom\n"
	<< "4 - Go upstairs\n";
      cin >> hospitalChoice;
      cout << "\n";

    switch (hospitalChoice)
    {
        case 1:
            if (key == "yes")
            {
                cout << "There is no one here and all the drawers and cabinets have been emptied.\n"
                << "On a tray next to the bed, there is an x-ray of a brain. There is something that looks like a bug lodged in it.\n";
            }
            else
            {
                cout << "You need a key to enter this room.\n";
            }
        break;
        case 2:
            cout <<"There is no one behind the desk. Maybe I can find something here.\n"
            << "You have found a key!\n";
            key = "yes";
            break;
        case 3:
            cout <<"You wash your face and look at your reflection in the mirror, wondering how this mess got started.\n";
            break;
    }   } while (hospitalChoice != 4);

    cout << "You have headed to the second floor\n\n"
      << "After walking up the stairs, you see a door that is barricaded. You walk over to it and knock on the door\n"
      << "A voice answers: 'Who's there?' You recognize that voice. It's your wife! She's alive!\n"
      << "You tell her that you have come to save her and start removing the barricade.\n"
      << "You then open the door and find your wife along with two other nurses. They are in bad shape. They have bites on their arms.\n"
      << "Enter any key to continue...";
      cin >> continue3;

    cout << "\n\nYou want to rescue them too, but you can't.\n"
         << "The four of you look at each other and know it is too late. There is nothing that can be done now.\n"
         << "One nurse speaks up and says: 'We will stay here. You guys should escape while you still can.'\n"
         << "You both nod and head for the exit.\nThe two of you get on the car and start driving to the next city, hoping that this nightmare has finally ended...\n\n";

    cout << "Congratulations! You have beat Mission Cops!\n"
         << "Would you like to play again? Enter 'y' for yes. Enter 'n' for no. ";
         cin >> replay;
 }
    cout <<"\nThank you for playing and we hope you enjoyed it.";
      return 0;
}
system ("pause");

return 0;


