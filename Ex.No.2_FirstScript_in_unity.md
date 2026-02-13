# Ex.No: 2  Welcome Script in Unity
### DATE:                                                                            
### REGISTER NUMBER : 
### AIM: 
 To learn the basic scripting in Unity and print welcome message in Console window. 
### Procedure:
1. Start the program
2. Open the Unity hub and Create a new 3D project
3. In Assets window, create the new folder and name it as Scripts
4. Create a new script with file name as FirstScript
5. Open the Script and print message "Welcome to Unity" inside the start function
6. Save the script
7. Create a new 3D game object in Hierarchy window and name it as 3DObject.
8. Add the component Firstscript in inspector window of 3Dobject.
9. Run the program
10. Stop the program.
### Program 
```
using System.Collections;
using System.Collections.Generic;
using UnityEngine;
public class FirstScript : MonoBehaviour
{
    // Start is called before the first frame update
    void Start()
    {
        print("Welcome to Unity");
    }

    // Update is called once per frame
    void Update()
    {
        
    }
}
```
### Output:
<img width="1317" height="747" alt="image" src="https://github.com/user-attachments/assets/90c5fd95-8036-46de-b694-881fe0d70ab0" />
<img width="1322" height="810" alt="image" src="https://github.com/user-attachments/assets/88c4cf2c-2bd9-4bf5-b4cd-cacb59a2a41c" />
<img width="1316" height="735" alt="image" src="https://github.com/user-attachments/assets/78201373-4ecf-4d71-aa2d-87ac22b7c2d2" />



### Result:
Thus the welcome script was printed on Console Window  sucessfully.

