## Force

I am sure you must have heard a lot about the term "Force" not only here but also in your high school "Physics Fundamentals" subject🤷🏻‍♂️ 
Guess Newton's laws of motion might come in handy✅
  </br>
  
![Force](https://media.giphy.com/media/oCQBxiSkYOvT2/giphy.gif)

As Newton’s Second Law, we know that (**Force= mass of the object * acceleration**). When force is applied to a body, it causes motion or a change. Force exists because of the interaction among the objects. 

In Unity, it works the same way. We can add a force to a RigidBody by using AddForce(). There are multiple ways in which you can use AddForce().

 

1. **AddForce**([Vector3](https://docs.unity3d.com/ScriptReference/Vector3.html) **force**, [ForceMode](https://docs.unity3d.com/ScriptReference/ForceMode.html) **mode**=ForceMode.Force);
    
    Parameters:
    
    - force: it is a Force vector in the world coordinates.
    - mode: It is a type of force that we can apply which would change to the Acceleration, Velocity, Impulse of a body.
2. **AddForce**(float **x**, float **y**, float **z**, [ForceMode](https://docs.unity3d.com/ScriptReference/ForceMode.html) **mode**=ForceMode.Force);
    - In the first way, we could see the first parameter is a force vector in the world coordinates. Now, what is world coordinates? It’s nothing but x,y, and z coordinate. You can also add them individually as the first parameter for the force vector.

*Note: Use Force functions in FixedUpdate() in Unity rather than in Update(). Because, Unity does the physics calculations much better in FixedUpdate(). We will look into FixedUpdate() later on in detail.*

Let’s look into the modes of force now. There are 4 types of modes available in Unity.

- ForceMode.Force: It applies a consistent force on the object. The effect depends on the simulation step length and the mass of the body.
- ForceMode.Impulse: It applies a quick striking force on the object. The effect depends on the mass of the body
- ForceMode.Acceleration: It specifies what acceleration you'd like the body to have at the current frame. The effect depends on the simulation step length but doesn't depend on the mass of the body.
- ForceMode.VelocityChange: It applies a direct velocity change, and changes the velocity by the value of force.

You can play around with all these functions and modes in your project to see how each and every object behaves.
