# Game-Dev---Unity---Heli Heli---MobileGame
Indie Game Development Three King Studios 
##### Collaborators: #####
Joseph E Powell IV 
* Software Engineeer/Programmer 
* Game Designer
* Artist

</br>
Joshua E Powell 
* Software Engineer/Programmer
* Game Developer
* Writer
</br>


# Heli Heli#

https://user-images.githubusercontent.com/47085746/145687972-ce5b2be8-0785-4a46-97e5-25604cd40c29.mp4


A mobile app game my twin brother and I was developing in the game engine called Unity. We got the inspiration from the mobile app game called Flappy Bird. This was a personal project of ours through our journey of game development. As of now we're both proficent in Unity, Unreal Engine 4, and Godot. We had taken tutorial courses online through Udemy whiched gave us the knowledge and skills to make better Unity games for mobile and pc. We made it to version 3.2, however the project was discontinued because we were more focused on BCT and school.
 
 
## Key Takeaways ##

 * Patience
 * Discipline
 * Problem Solving
 </br>
 
 

```
private void OnCollisionEnter2D(Collision2D collision)
    {
        if (collision.gameObject.CompareTag("Ground") ||
            collision.gameObject.CompareTag("Obstacles"))
        {
            //GameOver
            Time.timeScale = 0;
            replayBtn.SetActive(true);
            

        }
```
        
This sample code displayed above would execute the "Gameover" function when the Helicopter (ie player) comes into contact with an object resulting in the player's death and ends the game. 




```
 void Update()
    {
        if(timer > maxTime)
        {
            GameObject newobstacles = Instantiate(obstacles);
            newobstacles.transform.position = transform.position + new Vector3(0, Random.Range(-height, height), 0);
            Destroy(newobstacles, 15);
            timer = 0;
        }

        timer += Time.deltaTime;
    }

```

This sample code shown above executes the random spawning and placements of obstacles that the player had to avoid.




```
public class Move : MonoBehaviour
{
    public float speed;

    // Start 
    void Start()
    {

    }

    // Update is called once per frame
    void Update() => transform.position += Vector3.left * speed * Time.deltaTime;
}

```

The sample code above executes the movement of the spawning obstacles to move towards the player as soon as the game is started. The code that projects the Heli (Player) forward is the same as well but with the simple change of Vector3.right. 



### Update ###
Currently both Joseph and myself have learned to make games in Unity and Unreal Engine 4. We have decided to discontinue the project but take the experience we gained and apply it to future game development projects. We're currently trying to master Blender, Photoshop, and Animator to hone our 2D and 3D modeling skills and designs for better game assets. We are both proficient in programming languages such as C++, Java, Python, and C#. We are already working on a 3d gaming project. 













