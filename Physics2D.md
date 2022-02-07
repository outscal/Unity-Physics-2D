# Unity Physics 2D

Imagine a game that has no movements of players and enemies its just few blocks that are static, it would be such a dull game if we can’t interact with our player and enemies right??!! 😢 

That’s where Physics comes into action. In Unity using Physics we can add a force to a game object to make it move when it pushed by the player or hit, we can add velocity to it, we can play around with gravity and a lot of other stuff can be done. These are all things that we see in real life that we can implement in Unity.

Some of the main components of Physics are :

1. Colliders
2. Triggers
3. Rigidbody
4. Raycasts

Colliders : 

- As the name suggest colliders, in Unity helps a lot in detecting collision between game objects.
- In order for collisions to take place game objects must have Rigidbody component attached to it
- Colliders restrict the game objects from passing a certain point for eg : using colliders we can restrict our player to be enclosed within a room surrounded by 4 walls. We can use the same method to break a box when it collides with a bullet fired by the player or by a punch landed by the player.
- There are many other use cases of colliders in a game. 

    </br>

    ![Coll_1.png](https://github.com/outscal/Unity-Physics-2D/blob/main/Images/Coll_1.png?raw=true)
    


In the above snapshot we have added collider to our player as well as our platform due to which the platform restricts the player from passing through it and the player stays on it.

There are some functions that are used when colliders are interacting with other game objects:

1. [OnCollisionEnter2D](https://docs.unity3d.com/ScriptReference/MonoBehaviour.OnCollisionEnter2D.html) : This function gets called when a game object enters into collision.

    </br>

    ![Coll_enter.png](https://github.com/outscal/Unity-Physics-2D/blob/main/Images/Coll_enter.png?raw=true)
    
2. [OnCollisionExit2D](https://docs.unity3d.com/ScriptReference/MonoBehaviour.OnCollisionExit2D.html) : This function gets called when a game object exits collision.

    </br>

    ![coll_exit.png](https://github.com/outscal/Unity-Physics-2D/blob/main/Images/coll_exit.png?raw=true)
    
3. [OnCollisionStay2D](https://docs.unity3d.com/ScriptReference/MonoBehaviour.OnCollisionStay2D.html) : This function gets called when a game object stays in collision.

    </br>

    ![coll_stay.png](https://github.com/outscal/Unity-Physics-2D/blob/main/Images/coll_stay.png?raw=true)
    

There are other Collider 2D types that can be used with **Rigidbody** 2D as well:

- [Circle Collider 2D](https://docs.unity3d.com/Manual/class-CircleCollider2D.html) for circular collision areas.
- [Box Collider 2D](https://docs.unity3d.com/Manual/class-BoxCollider2D.html) for square and rectangle collision areas.
- [Polygon Collider 2D](https://docs.unity3d.com/Manual/class-PolygonCollider2D.html) for freeform collision areas.
- [Edge Collider 2D](https://docs.unity3d.com/Manual/class-EdgeCollider2D.html) for freeform collision areas and areas which aren’t completely enclosed (such as rounded convex corners).
- [Capsule Collider 2D](https://docs.unity3d.com/Manual/class-CapsuleCollider2D.html) for circular or lozenge-shaped collision areas.
- [Composite Collider 2D](https://docs.unity3d.com/Manual/class-CompositeCollider2D.html) for merging **Box Collider** 2Ds and Polygon Collider 2Ds.

Triggers :

- In the above section we have talked about how we want to restrict the player from passing through the game object.
- In this part we will be talking about how to enable the player from passing through a game object. Basically it is done using “is trigger” checkbox in the collider component.

    </br>

    ![Trigger.png](https://github.com/outscal/Unity-Physics-2D/blob/main/Images/Trigger.png?raw=true)
    
- When we check the “is trigger” component of a collider we disable the physics being applied to the component, which enables other game objects to pass through it still making it act as a collider.
- Triggers are mainly used for tutorials in games, in game collectables and also for level complete actions.
- Just like colliders, triggers also work on functions very similar to that of colliders as mentioned above.
    1. [OnTriggerEnter2D](https://docs.unity3d.com/ScriptReference/MonoBehaviour.OnTriggerEnter2D.html)
    2. [OnTriggerExit2D](https://docs.unity3d.com/ScriptReference/MonoBehaviour.OnTriggerExit2D.html)
    3. [OnTriggerStay2D](https://docs.unity3d.com/ScriptReference/MonoBehaviour.OnTriggerStay2D.html)

Rigidbody : 

- Rigidbodies are components that allow a GameObject to react to **real-time physics**. This includes reactions to forces and gravity, mass, drag and momentum.
- You can attach a Rigidbody to your GameObject by simply clicking on **Add Component** and typing in Rigidbody2D in the search field.

    </br>

    ![RB.png](https://github.com/outscal/Unity-Physics-2D/blob/main/Images/RB.png?raw=true)
    
- You will see that a new row of **RigidBody 2D** features is added in the inspector **view, just below the Transform component.

    </br>

    ![RB_1.png](https://github.com/outscal/Unity-Physics-2D/blob/main/Images/RB_1.png?raw=true)
    
- If we play our game now you will see that our game object drops down due to the gravity which looks no fun. To rectify this we can simply change the Gravity scale from 1 from 0.

    </br>

    ![Rb_2.png](https://github.com/outscal/Unity-Physics-2D/blob/main/Images/Rb_2.png?raw=true)
    
- By changing the gravity scale of that Rigidbody, you're basically defining how much the object is affected by gravity. In fact, try changing around the mass and gravity scale to different values and see what happens. The object still has a mass, it just doesn't care for the forces of gravity acting on it, and thus remains where it is.
- We can explore many other things by changing their values and noticing how the game object reacts.

Raycasts :

- A Raycast is like a laser beam fired from a point that we call as “Origin” along a particular direction to detect if our game object is still in collision with the other game object and if it is not in collision we perform certain operations.
- The big advantage is that every object which makes contact with the laser beam can be reported/detected.

    </br>

    ![Patrolling_enemy_raycast.png](https://github.com/outscal/Unity-Physics-2D/blob/main/Images/Patrolling_enemy_raycast.png?raw=true)
    
- In the above code, RaycastHit2D returns information about an object detected by a raycast in 2D physics. The RaycastHit2D class is used by [Physics2D.Raycast](https://docs.unity3d.com/ScriptReference/Physics2D.Raycast.html) and other functions to return information about the objects detected within the range fired by raycasts. 👾