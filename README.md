# airbnb-api
## V1 Inscription et Connexion
**Creation de la route sign_up**  
La route "/user/signup" permettra de créer un nouvel utilisateur en BDD. On vérifiera que l'email et le username transmis ne sont pas déjà présents en BDD, et que tous les paramètres (password, email, username, name, description) ont bien été renseignés lors de la création du nouveau compte.
À chaque utilisateur sera associé un token (identifiant unique).
Le password transmis sera encrypté en base de données grâce à un hash et un salt.

**Creation de la route login**  
La route "/user/login" permettra à l'utilisateur de se connecter.
On vérifiera que l'email et le password ont été transmis, puis que l'identifiant (email) est présent en BDD.
On vérifiera ensuite que le password renseigné correspond au password encrypté en BDD.
