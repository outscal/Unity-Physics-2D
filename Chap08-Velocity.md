## Velocity

We know that velocity is the rate of change of an object’s position. In Unity, when you add rigidbody to a game object and apply velocity, it works the exact same way as that of its definition. It represents the rate of change of Rigidbody position.

        public Rigidbody2D rb;

        void Start()
        {
            rb = GetComponent<Rigidbody>();
        }

        voidFixedUpdate()
        {
                rb.velocity = newVector2(0, 5);
        }

---

<aside>

> 💡 🚀 **[Join Discord Server](https://discord.gg/J5zDscnzms) → Get your doubts solved by experts instantly**

</aside>

![discord](./Images/discord.png)

---
