## Gravity

Take an object having mass and throw it in the sky. The object will fall down to the earth’s surface. Hence, gravity is a force that attracts physical particles down towards the center of the earth’s surface. 

Unity’s physics system works in a similar way. Put a game object in the scene having the rigidbody component attached to it and don’t put any other game object. Play it. You will observe that the game object is falling down on the -y axis.

Well, you can play around with the y axis coordinate values in the Vector function.

```jsx
Physics.gravity = new Vector2(0,-1.0f);
```

You can also use “useGravity” in the scripts. It controls whether gravity should affect a body or not. Note: It will work only when the game object is attached a rigidBody component to it.


---

<aside>

> 💡 🚀 **[Join Discord Server](https://discord.gg/J5zDscnzms) → Get your doubts solved by experts instantly**

</aside>

![discord](./Images/discord.png)

---