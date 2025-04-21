# Bot Battlr 🤖⚔️  
**A Galactic Bot Army Management System**  

![Bot Battlr Demo](demo.gif) <!-- Add demo GIF/Image post-setup -->

## 🚀 Table of Contents  
- [Overview](#-overview)  
- [Features](#-features)  
- [Tech Stack](#-tech-stack)  
- [Setup Guide](#-setup-guide)  
- [Data Structure](#-data-structure)  
- [Component Architecture](#-component-architecture)  
- [API Documentation](#-api-documentation)  
- [Contributing](#-contributing)  
- [Troubleshooting](#-troubleshooting)  
- [License](#-license)  

---

## 🌌 Overview  
As the **Galactic Overlord**, you need an army of bots to conquer the universe. **Bot Battlr** lets you:  
- **Browse** all available bots  
- **Enlist** bots into your army  
- **Release** bots from duty  
- **Discharge** bots permanently (they'll be *deleted from the galaxy!*)  

Built with React, this app demonstrates:  
✅ Component-based architecture  
✅ State/props management  
✅ Data fetching from a local JSON server  
✅ Event handling  

---

## ✨ Features  
| Feature | Description |  
|---------|-------------|  
| **Bot Collection** | View all bots with stats (health, damage, class) |  
| **Enlist/Release** | Add/remove bots from your army with one click |  
| **Permanent Discharge** | Delete bots forever (both UI and backend) |  
| **Responsive UI** | Works on desktop and mobile devices |  
| **Real-time Updates** | Army updates instantly without page refresh |  

---

## 💻 Tech Stack  
- **Frontend**:  
  ![React](https://img.shields.io/badge/React-18.2.0-blue)  
  ![React Router](https://img.shields.io/badge/React_Router-6.15.0-orange)  
- **Backend**:  
  ![JSON Server](https://img.shields.io/badge/JSON_Server-0.17.3-green)  
- **Styling**: Plain CSS  

---

## 🛠️ Setup Guide  

### Prerequisites  
- Node.js ≥16.0.0  
- npm ≥7.0.0  

### Steps  
1. **Clone the Repository**:  
   ```bash  
   git clone https://github.com/your-username/bot-battlr.git  
   cd bot-battlr  

2. **Install Dependencies**:

```bash
npm install
```
3. **Set Up Local JSON Server**:

```bash
npm install -g json-server 
``` 
3. **Create a db.json file**
 Create a `db.json file` in the root directory .
Start the Backend Server (in a new terminal):

```bash
json-server --watch db.json --port 3001 
``` 
4. **Start the React App**:

```bash
npm start  
Open in Browser:
Visit http://localhost:3000
```
5. **🗃️ Data Structure
Sample db.json file**:

```json
{
  "bots": [
    {
      "id": 186,
      "name": "G-17",
      "health": 50,
      "damage": 20,
      "armor": 98,
      "bot_class": "Defender",
      "catchphrase": "1001111001000111010111110010111101111",
      "avatar_url": "https://robohash.org/isteaeos.png?size=300x300&set=set1",
      "created_at": "2018-10-02T19:55:12.348Z",
      "updated_at": "2018-10-02T19:55:12.348Z"
    },
    {
      "id": 188,
      "name": "]W-40",
      "health": 80,
      "damage": 35,
      "armor": 75,
      "bot_class": "Captain",
      "catchphrase": "001010010010111000011110101111000110111010",
      "avatar_url": "https://robohash.org/doloribusetsint.png?size=300x300&set=set1",
      "created_at": "2018-10-02T19:55:12.378Z",
      "updated_at": "2018-10-02T19:55:12.378Z"
    } 
  ]  
}  
```
## 🧩 Component Architecture
```list
src/  
├── App.js              
├── components/  
│   ├── BotCard.js  
│   ├── BotCollection.js  
│   |── YourBotArmy.js
|   |── BotSpecs.js
|   |── BotPage.js
```  
### Data Flow
1. **App** fetches bots from `/bots` endpoint.

2. **BotCollection** receives bots via props and renders `BotCard` components.

3. **YourBotArmy** manages enlisted bots using state.

4. **BotCard** handles enlist/release/discharge actions via props.

## 📡 API Documentation
**Endpoint**	**Method**	  **Description**
`/bots`	          GET	       Fetch all bots
`/bots/:id`	    DELETE	       Delete a bot

##### Example Request:

```bash
curl http://localhost:3001/bots 
``` 
## 🐛 Troubleshooting

**Issue**	                 **Solution**
*Bots not loading*	          Ensure JSON server is running on port 3001
*Enlist button not working*	  Check if bot is already in the army
*CORS errors*	              Verify both servers (React/JSON) are running

## 🤝 Contributing
1. Fork the repo.

2. Create a feature branch:

```bash
git checkout -b feat-awesome-bot  ,
```
3. Commit changes:

```bash
git commit -m "Add plasma cannon feature" 
``` 
4. Push to the branch:

```bash
git push origin feat-awesome-bot

```
5. Open a Pull Request

## 📜 License
MIT © 2023 Elvis