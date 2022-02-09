## Raycasts

- A Raycast is like a laser beam fired from a point that we call as “Origin” along a particular direction to detect if our game object is still in collision with the other game object and if it is not in collision we perform certain operations.
- The big advantage is that every object which makes contact with the laser beam can be reported/detected.

    </br>

    ``` cs
        public class Patrolling_Enemies : MonoBehaviour
        {
            public Transform originpoint; 
            Vector2 dir = new Vector2(-1, 0); 
            public float range; 
            public float speed;
            Rigidbody2D rb;

            void Start()
            {
                rb = GetComponent<Rigidbody2D>();
            }
            
            void Update()
            {
                RaycastHit2D hit = Physics2D.Raycast(originpoint.position, dir, range); 
                if(hit == false)
                {
                    Vector3 new_Scale = transform.localScale; 
                    new_Scale.x *= -1; 
                    transform.localscale = new_Scale; 
                    speed *= -1; 
                    dir *= -1;
                }
            }         
    ```
    
- In the above code, RaycastHit2D returns information about an object detected by a raycast in 2D physics. The RaycastHit2D class is used by [Physics2D.Raycast](https://docs.unity3d.com/ScriptReference/Physics2D.Raycast.html) and other functions to return information about the objects detected within the range fired by raycasts. 👾


---

<aside>

> 💡 🚀 **[Join Discord Server](https://discord.gg/J5zDscnzms) → Get your doubts solved by experts instantly**

</aside>

![discord](./Images/discord.png)

---
