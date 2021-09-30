# Lecture-7-Exercises-Slide-16-20-
Exercises in Lecture 7 (Slide 16-20)

// Mark my Words (Slide 16)

    #include <iostream>
    using namespace std;

    int main() {

      cout << "This Is a Program to Check the Grade Boundaries of a Test Paper\n\n"; // Outputs the title of the program.
      cout << "Please enter the grade of the paper\n"; // Asks the user to input the grade of the paper

      int grade;
      cin >> grade; // User inputs grade of the paper

      if (grade >= 70) { // Executed if user inputs a grade equal to or more than 70

        cout << "\nThe Grade of the Paper is: A\n";
        cout << "This student has done an excellent job in this subject!\n";

      }

      else if (grade >= 60 && grade <= 69) { // Executed if user inputs a grade within 60-69

        cout << "\nThe Grade of the Paper is: B\n";
        cout << "This student has done a good job in this subject!\n";

      }

      else if (grade >= 50 && grade <= 59) { // Executed if user inputs a grade within 50-59

        cout << "\nThe Grade of the Paper is: C\n";
        cout << "This student has done a satisfactory job in this subject!\n";

      }

      else if (grade >= 40 && grade <= 49) { // Executed if user inputs a grade within 40-49

        cout << "\nThe Grade of the Paper is: D\n";
        cout << "The student has done an unsatisfactory job in this subject.\n";

      }

      else { // Executed if user inputs a grade below 40

        cout << "\nThe Grade of the Paper is: F\n";
        cout << "The student has failed the subject.\n";

      }
      cin.get();
      return 0;
    }
    
    
// Starting a Band (Slide 17-18)
    
    #include <iostream>
    #include <string>
    using namespace std;

    int main() {

        cout << "This Program Will Check If Your Friend Is Eligible to Enter the Band and If You Can Start a Band!\n\n"; // Outputs the title of the program
        bool musicalFriend = true;
        string friendPlays = "guitar";
        string friendPlays2 = "drums";

        bool musicalFriendin;
        string friendPlaysin;

        cout << "Is your friend talented at music? (Write 0 if No, Write 1 if Yes)\n"; // Asks the user if the friend is talented at music
        cin >> musicalFriendin; // User inputs answer


        if (musicalFriend == musicalFriendin) { // If the user is a musical friend this will execute

            cout << "What instrument does your friend play? (Please type in lowercase only)\n"; // Asks the user what instrument the friend plays
            cin >> friendPlaysin; // User inputs instrument

            if (friendPlaysin == friendPlays || friendPlaysin == friendPlays2) { // If the user plays guitar or drums this will execute

                cout << "\nCongratulations, your friend can enter the band!\n";
                cout << "You can start a band!\n";

            }

            else { // If the user plays a instrument other than guitar or drums this will execute

                cout << "\nAww... Sorry, we don't accept the instrument your friend is using for the band.\n"; 
                cout << "You can't start a band.\n";
            }

        }

        else { // If the user is not a musical friend this will execute

            cout << "\nAww... Sorry, we only allow musical friends in the band.\n";
            cout << "You can't start a band.\n";
        }
        cin.get();
        return 0;
    }
    
   
// Killing Time (Slide 19)

    #include <iostream>
    #include <string>
    using namespace std;

    int main() {

        cout << "This Program Will Check What to Do in Situations That You're Killing Time in Dubai Mall.\n\n"; // Outputs the title of the program.

        cout << "How many minutes do you have left till your friend arrives with you in Dubai Mall?\n"; // Asks the user how many minutes does the friend have till he arrives,
        int time;
        cin >> time; // User inputs time


        if (time >= 15) { // Executed if time is more than or equal to 15

            cout << "How much money do you have in your pocket?\n"; // Asks the user how much money does he have.
            double money;
            cin >> money; // User inputs money

            if (money > 5) { // Executed if money is more than 5
                cout << "\nGo buy a coffee!\n";


                    cout << "\nNow pick a coffee to choose!\n"; // Added a creative twist to the task wherein the user will then pick what coffee to choose.
                    cout << "\nYour favorite coffees are either: latte or cappuccino (please type in lowercase only)\n"; // Asks user what coffee to choose between Latte or Cappuccino.
                    string coffee;
                    cin >> coffee; // User inputs the coffee

                    if (coffee == "latte") { // Executed if user types latte

                        cout << "\nThe best Latte in Dubai Mall is definitely in Costa Coffee! Go to the ground floor to buy one.\n";
                        cout << "\nCosta Coffee's  aromatic Espresso and creamy milk come together beautifully in their Latte. This pair is perfect for those who prefer their drinks hot in the winter and cool in the summer.\n";

                        }

                    else if (coffee == "cappuccino") { // Executed if user types cappuccino

                        cout << "\nThe best Cappuccino in Dubai Mall is definitely in Starbucks! Go to the first floor to buy one.\n";
                        cout << "\nUnder a smoothed and stretched layer of thick foam, Starbucks' extremely smooth and delicately sweet Espresso awaits. With a silky, frothy foam and a sharp, chilly undercurrent, this Cappuccino has a luscious mouthfeel.\n";

                    }
                    else { // Executed if user didn't type it correctly or chose another coffee
                        cout << "\nThe coffee you picked is not one of your favorites! Please pick either Latte or Cappuccino.\n";
                    }


            }

            else { // Executed if money is less than 5

                cout << "\nGo for a walk around the town!\n"; 

                    cout << "\nNow pick a direction to walk!\n";  // Added a creative twist to the task wherein the user will then pick what direction to go.
                    string direction;
                    cout << "\nleft or right? (please type in lowercase only)\n"; // Asks the user if the direction is left or right.
                    cin >> direction; // User inputs the direction.

                    if (direction == "left") { // Executed if user inputs left

                        cout << "\nAt your left, you will see the Dubai Aquarium\n"; 
                        cout << "\nOver 33,000 marine species are on display at the Dubai Aquarium. Staring at the diverse fishes and other aquatic animals is a visual feast.\n";

                    }

                    else if (direction == "right") { // Executed if user inputs right

                        cout << "\nAt your right, you will see the Human Waterfalls.\n";
                        cout << "\nThe Human Waterfalls is a beautiful water structure that will have observers marveling at the water falls. It is frequently utilized as a meeting point for mall visitors.\n";
                    }

                    else { // Executed if user didn't type it correctly or chose another direction
                        cout << "\nWhere are you going? You can only go left or right.\n";

                    }



            }


        }
        else { // Executed if time is less than 15

            cout << "\nSit in the food zone and wait.\n";

        }
        cin.get();
        return 0;
    }

    
// Earthquake (Slide 20)

    #include <iostream>
    using namespace std;

    int main() {


      cout << "This Program Reads the Magnitude From the User Under the Richter Scale and Displays an Appropriate Descriptor to It.\n\n"; // Outputs the title of the program.


      cout << "To get started, please enter the magnitude of the earthquake\n"; // Asks the user to input the magnitude of the earthquake.
      double magnitude;

      cin >> magnitude; // User inputs magnitude

      if (magnitude < 10.0) { // Executed if magnitude is less than 10.0

        if (magnitude < 2.0) { // Executed if magnitude is less than 2.0
          cout << "\nThe earthquake's magnitude is micro.\n";
          cout << "During such earthquake, people aren't usually aware of it, even if it's recorded on local instruments.\n";
        }
        else if (magnitude >= 2.0 && magnitude < 3.0 ) { // Executed if magnitude is between 2.0 to 2.9
          cout << "\nThe earthquake's magnitude is very minor.\n";
          cout << "In this earthquake, some people have a small sense of it and no structural damage.\n";
        }

        else if (magnitude >= 3.0 && magnitude < 4.0) { // Executed if magnitude is between 3.0 - 3.9
          cout << "\nThe earthquake's magnitude is minor.\n";
          cout << "People are often aware of it, yet it rarely does harm. The swaying of indoor objects can be felt.\n";
        }
        else if (magnitude >= 4.0 && magnitude < 5.0) { // Executed if magnitude is between 4.0 - 4.9
          cout << "\nThe earthquake's magnitude is light.\n";
          cout << "Interior things shake and creaking noises are audible. Most people in the affected area are aware of it. In most cases, there is no or limited injury.\n";
        }
        else if (magnitude >= 5.0 && magnitude < 6.0) { // Executed if magnitude is between 5.0 - 5.9
          cout << "\nThe earthquake's magnitude is moderate.\n";
          cout << "Can inflict varied degrees of damage to poorly designed structures. All other structures suffered minor to no damage. Everyone can sense it.\n";
        }
        else if (magnitude >= 6.0 && magnitude < 7.0) { // Executed if magnitude is between 6.0 - 6.9
          cout << "\nThe earthquake's magnitude is strong.\n";
          cout << "A moderate number of well-built structures in inhabited regions can be damaged. Wider areas are affected, extending hundreds of kilometers from the epicenter. In the epicentral area, there is strong to intense shaking.\n";
        }
        else if (magnitude >= 7.0 && magnitude < 8.0) { // Executed if magnitude is between 7.0 - 7.9
          cout << "\nThe earthquake's magnitude is major.\n";
          cout << "Most buildings are damaged, with some partially or totally collapsing or receiving serious damage. Major damage is primarily limited to 250 kilometers from the epicenter, however it can be felt over a wide area.\n";
        }
        else if (magnitude >= 8.0 && magnitude < 10.0) { // Executed if magnitude is between 8.0 - 9.9
          cout << "\nThe earthquake's magnitude is great.\n";
          cout << "Buildings have suffered significant damage, and structures are likely to be demolished. Large-scale destruction. Extremely large areas are affected.\n";
        }
      }	
      else { // Executed if magnitude is equal to or more than 10.0
        cout << "\nThe earthquake's magnitude is meteoric.\n";
        cout << "All buildings have been severely damaged or collapsed, resulting in entire or near-total destruction. Changes in the topography of the ground are permanent.\n";
      }

      cout << "\n\nSource: Wikipedia Contributors (2021) Richter Magnitude Scale. [online] En.wikipedia.org. Available at: <https://en.wikipedia.org/wiki/Richter_magnitude_scale> [Accessed 30 September 2021].\n"; // Outputs the source used in writing the magnitude.

      cin.get();
      return 0;
    } 
