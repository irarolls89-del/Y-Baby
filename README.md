<!DOCTYPE html><html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>YA BABY – Casino Dice 4 Players</title>
<style>
/* Full CSS from the final version, including avatars, dice, sparkles, fireworks */
body{margin:0;font-family:Arial;background:#000;color:#fff;text-align:center;position:relative;}
h1{text-shadow:0 0 12px crimson;margin-top:12px;}
#table{max-width:800px;margin:auto;padding:24px;background:radial-gradient(circle,#0e3b2c,#020);border-radius:28px;box-shadow:0 0 50px crimson;border:2px solid #800;position:relative;z-index:1;}
#top-players,#bottom-players{display:flex;justify-content:space-between;margin:16px 0;}
.player-container{display:flex;flex-direction:column;align-items:center;position:relative;}
.player-avatar{width:60px;height:60px;border-radius:50%;border:2px solid gold;display:flex;align-items:center;justify-content:center;font-weight:bold;color:#fff;font-size:20px;margin-bottom:4px;transition: transform 0.2s, box-shadow 0.2s;}
.player-avatar.active{transform: scale(1.2);box-shadow:0 0 20px gold;animation: bounce 0.6s infinite;}
.player-avatar.winner{animation: winnerPulse 1s infinite alternate;box-shadow:0 0 30px gold,0 0 50px gold inset;}
@keyframes bounce{0%,100%{transform:scale(1) translateY(0);}50%{transform:scale(1.2) translateY(-8px);}}
@keyframes winnerPulse{0%{transform:scale(1.2) rotate(0deg);}50%{transform:scale(1.35) rotate(5deg);}100%{transform:scale(1.2) rotate(0deg);}}
.player-name{font-size:14px;font-weight:bold;color:#fff;}
#dice{display:grid;grid-template-columns:repeat(6,1fr);gap:12px;margin:0 auto;position:relative;}
.die{font-size:48px;background:linear-gradient(145deg,#444,#222);color:#fff;border-radius:16px;padding:24px 0;cursor:pointer;box-shadow:0 0 10px #000 inset,0 0 20px crimson;transition:all 0.2s;}
.held{background:gold;color:#000;box-shadow:0 0 16px gold,0 0 30px gold inset;animation: glow 1s infinite alternate;}
@keyframes glow{0%{box-shadow:0 0 16px gold,0 0 30px gold inset;}100%{box-shadow:0 0 32px gold,0 0 60px gold inset;}}
#table button{font-size:16px;padding:10px 20px;margin:4px;border:none;border-radius:12px;background:crimson;color:#fff;cursor:pointer;transition:0.2s;}
#table button:hover{background:#f00;}
#status{min-height:26px;font-weight:bold;font-size:16px;}
#scoreboard{margin-top:16px;background:#111;padding:12px;border-radius:14px;text-align:left;}
.score{display:flex;justify-content:space-between;cursor:pointer;padding:4px 0;}
.used{opacity:.5;text-decoration:line-through;}
#winner{font-size:22px;color:# Y-Baby