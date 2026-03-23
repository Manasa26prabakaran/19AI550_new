# Ex.No: 10  Implementation of 2D/3D game -------------------
### DATE:                                                                            
### REGISTER NUMBER : 212224230149
### AIM: 
To develop a 3D Roller Ball game using Unity with AI-based agent behavior.
### Algorithm:
```
Open Unity Hub and create a new 3D project.
Create a plane to act as the ground surface.
Add a sphere object to represent the player (roller ball).
Attach Rigidbody and Collider components to enable physics.
Add collectible objects (cubes) in the scene.
Write a C# script to control the movement of the ball.
Implement collision detection to collect objects.
Integrate AI behavior using Unity ML-Agents or simple scripted logic.
Train or program the agent to collect objects efficiently.
Test the game and ensure proper interaction between objects.
Debug errors and optimize performance.
Build and run the game.
```  
### Program:
```
Player Controller Script:
using UnityEngine;

public class PlayerController : MonoBehaviour
{
    public float speed = 10.0f;
    private Rigidbody rb;
    private int count;

    void Start()
    {
        rb = GetComponent<Rigidbody>();
        count = 0;
    }

    void FixedUpdate()
    {
        float moveHorizontal = Input.GetAxis("Horizontal");
        float moveVertical = Input.GetAxis("Vertical");

        Vector3 movement = new Vector3(moveHorizontal, 0.0f, moveVertical);
        rb.AddForce(movement * speed);
    }

    void OnTriggerEnter(Collider other)
    {
        if (other.gameObject.CompareTag("PickUp"))
        {
            other.gameObject.SetActive(false);
            count = count + 1;
        }
    }
}
Simple AI Movement Script:
using UnityEngine;

public class AIController : MonoBehaviour
{
    public Transform target;
    public float speed = 5f;

    void Update()
    {
        transform.position = Vector3.MoveTowards(transform.position, target.position, speed * Time.deltaTime);
    }
}
```
### Output:

### Result:
Thus the game was developed using Unity and adopted _-----------AI technology.
