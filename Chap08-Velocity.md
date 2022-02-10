## Velocity

Great!!! you are one step away from completing your Unity Physics course 😎
Welcome to the final chapter of Unity Physics!!!! 🎉🎉

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

