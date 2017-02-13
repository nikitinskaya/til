switch/case is like else/else if, but neater

ex: equiv of the command line prompt to acccept or decline

else/else if would also require OR, like input == y or input == Y (too long!)

switch(input)
{
  case 'y':
  case 'Y':
    cout << "yes\n";
    break;
  
  case 'n':
  case 'N':
    cout << "no\n";
    break; 
    
  default:
    cout << "wtf?\n";
    break; 
}


break only takes us out of the switch thing, but not out of a cycle, if the switch is inside one
