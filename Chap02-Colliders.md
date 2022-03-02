## Colliders 

- Great!!!! you are all set on understanding what Unity Physics is all about 😎
- Ever wondered how a car flips in GTA once you dash into another car?? 🤔🤔 That's where Colliders come in action.
- As the name suggest colliders, in Unity helps a lot in detecting collision between game objects.

    <br>

![collision](https://media.giphy.com/media/xTiTnzwJoXpg7gdONy/giphy.gif)

- In order for collisions to take place game objects must have Rigidbody component attached to it
- Colliders restrict the game objects from passing a certain point for eg : using colliders we can restrict our player to be enclosed within a room surrounded by 4 walls. We can use the same method to break a box when it collides with a bullet fired by the player or by a punch landed by the player.
- There are many other use cases of colliders in a game. 

    <br>

![Coll_1.png](https://github.com/outscal/Unity-Physics-2D/blob/main/Images/Coll_1.png?raw=true)
    


In the above snapshot we have added collider to our player as well as our platform due to which the platform restricts the player from passing through it and the player stays on it.

    

There are other Collider 2D types that can be used with **Rigidbody** 2D as well:

- [Circle Collider 2D](https://docs.unity3d.com/Manual/class-CircleCollider2D.html) for circular collision areas.
- [Box Collider 2D](https://docs.unity3d.com/Manual/class-BoxCollider2D.html) for square and rectangle collision areas.
- [Polygon Collider 2D](https://docs.unity3d.com/Manual/class-PolygonCollider2D.html) for freeform collision areas.
- [Edge Collider 2D](https://docs.unity3d.com/Manual/class-EdgeCollider2D.html) for freeform collision areas and areas which aren’t completely enclosed (such as rounded convex corners).
- [Capsule Collider 2D](https://docs.unity3d.com/Manual/class-CapsuleCollider2D.html) for circular or lozenge-shaped collision areas.
- [Composite Collider 2D](https://docs.unity3d.com/Manual/class-CompositeCollider2D.html) for merging **Box Collider** 2Ds and Polygon Collider 2Ds.

