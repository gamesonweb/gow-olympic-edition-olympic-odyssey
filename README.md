# Olympic Odyssey

## Overview
Welcome we're excited to develop an innovative game that combines management, 
4X and adventure elements, all set in the thrilling world of the Olympic Games for the Games On Web tournament. 
Inspired by the game [For the King](https://store.steampowered.com/app/527230/For_The_King/) and [Baldur's Gate III](https://store.steampowered.com/app/1086940/Baldurs_Gate_3/) for the gameplay.

- [Repository Github](https://github.com/Tit0u4N/games-on-web-team-ficsit)
- [Video Presentation](TODO)
- [Team Members](#team-members)
- [Technology Stack](#technology-stack)
- [History, Details and Difficulties of the Development](#history-details-and-difficulties-of-the-development)
- [Development Approach](#development-approach)
  - [Package Management](#package-management)
  - [Getting Started](#getting-started)

## Team Members
- **[Titouan Lacombe--Fabre](https://github.com/Tit0u4N)** (L3 MIAGE, MIAGE Nice - Sophia)
- **[Tamas Palotas](https://github.com/Shiyamii)** (Bachelor degree in computer science *BUT 3*, Nice)
- **[Baptiste Lacroix](https://github.com/BaptisteLacroix)** (SI3 FISA, Diploma in computer engineering, Polytech Nice Sophia)

## Technology Stack
Our project is built using a robust and modern technology stack to ensure a high-quality gaming experience:

- **Primary Libraries:**
    - **BabylonJS**: For rendering stunning 3D graphics and creating immersive game environments.
    - **React**: To build a dynamic and responsive user interface.

- **Secondary Libraries:**
    - **NextUI**: For a modern and responsive UI design.
    - **Tailwind**: For sleek and efficient styling.
    - **SCSS**: To enhance CSS with more advanced styling capabilities.

- **Programming Language:** The entire project is written in **TypeScript**, utilizing its strong typing features for better code quality and maintainability.

- **Build Tool:** We use **Vite** for fast and efficient building and development.

- **Testing Framework:** We use **Jest** for testing our codebase.

- **Formatters and Linters:** We use **Prettier** and **ESLint** to ensure consistent code style and quality.

### The Idea
Pour créer le jeu nous voulions partir sur un type de jeux différents des autres.
Nous avons donc décidé de partir sur un jeu de gestion de ressources, de stratégie et d'aventure en s'inspirant de jeux comme For the King et Baldur's Gate III.
Nous avons imaginé un plateau de jeu en case hexagonale avec deux types de batimens dessus :
- Les centre d'entrainement qui permettent d'améliorer les compétences de nos athlètes
- Les arenes qui permettent de combattre d'autres équipes pour gagner des objets

Puis nous avons imaginé une compétitions final représentant les JO a la fin du jeux. Sous forme d'énorme tournois réunissant tout les sport.

## Point clé du développement
### Step 1 : Génération de la map
Pour génerer la map nous avons utilisée le bruit de perlin puis en addition un algorithm afin de donner une forme d'ile a notre map.
Pour cela nous avons utilisée une librairie nodeJS 'tumult' qui permet de générer des bruits de perlin.
Afin de pouvoir utiliser la librairie dans notre projet nous avons du encapsuler le code dans une class Noise en typescript.

<p align="center">
  <img src="./images/perlin_1.png" alt="Image bruit de perlin" width="35%" />
  <img src="./images/perlin_2.png" alt="Image bruit de perlin" width="55%" />
</p>

Afin de générer la map comme nous le souhaitions nous avons ajuster l'algorythme jusqu'a obtenir le résultat souhaité.

### Step 2 : Le dé
Le lancer de dé étant le coeur nous avons décidé de donner au joeuur deux possiblilié :
#### Lancement de dé 2D
Nous avons en premier lieux créer une facon de lancé le dé en 2D étant plus rapide.
<p align="center">
  <img src="./images/dice_2d.png" alt="Image bruit de perlin" width="80%" />
</p>






## Development Approach
Our development follows the **Model-View-Presenter (MVP)** architecture. This approach allows us to separate the logic, UI, and data handling aspects of the project, making our code more modular, scalable, and easier to manage.

### Package Management
We use **Yarn** as our package manager. The following commands are essential for working with our project:

- `yarn install`: To install all the necessary dependencies.
- `yarn run dev`: To start the development server.
- `yarn build`: To build the project for production.
- `yarn test`: To run the test suite.
- `yarn format`: To run the code formatter.

### Getting Started
To get started with contributing to this project, please follow these steps:

1. Clone the repository.
2. Run `yarn install` to install all dependencies.
3. Create a new branch for your feature following the naming convention.
4. Develop your feature and commit your changes.
5. Push your branch and open a pull request for review.
