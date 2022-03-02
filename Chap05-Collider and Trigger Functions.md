# Collider and Trigger Functions

You've learnt about colliders and triggers till now. 

![Congrats](https://media.giphy.com/media/3oz8xAFtqoOUUrsh7W/giphy.gif)

Here, you will learn about the functions used for the collision and triggering any object. 


First, let's see what are functions to be used for the collision.

1. [OnCollisionEnter2D](https://docs.unity3d.com/ScriptReference/MonoBehaviour.OnCollisionEnter2D.html) : This function gets called when a game object enters into collision.

    </br>

    ```cs
    
    void OnCollisionEnter2D(Collision2D collision)
    {
        //block of code to execute when game object enters into collision
    }

    ```
    
2. [OnCollisionExit2D](https://docs.unity3d.com/ScriptReference/MonoBehaviour.OnCollisionExit2D.html) : This function gets called when a game object exits collision.

    </br>

    ```cs
    
    void OnCollisionExit2D(Collision2D collision)
    {
        //block of code to execute when game object exits collision
    }

    ```
    
3. [OnCollisionStay2D](https://docs.unity3d.com/ScriptReference/MonoBehaviour.OnCollisionStay2D.html) : This function gets called when a game object stays in collision.

    </br>

     ```cs
    
    void OnCollisionStay2D(Collision2D collision)
    {
        //block of code to execute when a game object stays in collision
    }

    ```



Next, comes Trigger functions.

Just like colliders, triggers also work on functions very similar to that of colliders as mentioned above.

1. [OnTriggerEnter2D](https://docs.unity3d.com/ScriptReference/MonoBehaviour.OnTriggerEnter2D.html) This function gets called on another object which enters a trigger collider attached to current object.

    </br>

     ```cs
    
    void OnTriggerEnter2D(Collider2D collision)
    {
        //block of code to execute when another game object enters a trigger collider.
    }

    ```

2. [OnTriggerExit2D](https://docs.unity3d.com/ScriptReference/MonoBehaviour.OnTriggerExit2D.html) This function gets called on another object which leaves a trigger collider attached to current object.

    </br>

     ```cs
    
    void OnTriggerExit2D(Collider2D collision)
    {
        //block of code to execute when another game object exits a trigger collider.
    }

    ```

3. [OnTriggerStay2D](https://docs.unity3d.com/ScriptReference/MonoBehaviour.OnTriggerStay2D.html) This function gets called on each frame till the object leaves the trigger collider

    </br>

     ```cs
    
    void OnTriggerStay2D(Collider2D collision)
    {
        //block of code to execute when another game object stays in trigger collider.
    }

    ```
