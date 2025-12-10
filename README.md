# cloudVector
Heroku's lil brother.

i am not sure wether to make it cli based or gui basedBut cli based is a bit meaningless.
like it is supposed to deploy projects over our server and lay person cant do it using just cli.
ok so web interface is must for women and aslo a cli based package should be their for engineers isnt it?
now stack for backend will be django as always. i am finalizing stack for cli pckage.
it should either be just for static or both tatic and dynamic
builderpack works both with both static and dynamic stacks.



+----------------+           +-------------------+
| GUI (Web App)  |           | CLI (Python Tool) |
+-------+--------+           +---------+---------+
        |                          |
        | REST/GraphQL API          |
        +----------+----------------+
                   |
                   v
           +----------------+
           | Django Backend |
           +--------+-------+
                    |
        +-----------+------------+
        |                        |
+-------v-------+         +------v-------+
| Repo Manager  |         | Deployment   |
| (GitHub/Git)  |         | Manager      |
+-------+-------+         +------+-------+
        |                        |
        |                        |
   +----v----+            +------v-------+
   | Clone   |            | Static/Dynamic|
   | Repo    |            | Deployment    |
   +----+----+            +------+--------+
        |                        |
        |                        |
   +----v----+            +------v--------+
   | Detect   |           | Nginx / S3 /  |
   | Type     |           | Docker        |
   +----------+           +---------------+


