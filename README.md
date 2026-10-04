<html lang="ru">

<head>

<meta charset="UTF-8">

<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Открытка</title>

<style>

*{box-sizing:border-box}

html,body{margin:0;width:100%;height:100%;overflow:hidden}

body{

  background:#000;color:#fff;font-family:Arial,Helvetica,sans-serif;

  display:flex;align-items:center;justify-content:center;position:relative;

}

#hearts{position:fixed;inset:0;overflow:hidden;pointer-events:none;z-index:0}

.heart{

  position:absolute;top:-40px;color:#5b0909;

  text-shadow:0 0 7px #430000,0 0 15px rgba(120,0,0,.45);

  animation:fall linear forwards;opacity:.65

}

@keyframes fall{

  0%{transform:translateY(-50px) rotate(0deg);opacity:0}

  10%{opacity:.65}90%{opacity:.65}

  100%{transform:translateY(110vh) rotate(360deg);opacity:0}

}

.screen{position:relative;z-index:1;width:min(90vw,520px);text-align:center}

.card{

  background:rgba(10,10,10,.92);border:1px solid #2a2a2a;border-radius:18px;

  padding:34px 24px;box-shadow:0 0 30px rgba(90,0,0,.22);

}

.view{animation:enter .65s ease both}

.view.exit{animation:exit .35s ease both}

@keyframes enter{

  from{opacity:0;transform:translateY(22px) scale(.97);filter:blur(5px)}

  to{opacity:1;transform:translateY(0) scale(1);filter:blur(0)}

}

@keyframes exit{

  from{opacity:1;transform:translateY(0) scale(1)}

  to{opacity:0;transform:translateY(-18px) scale(.98);filter:blur(4px)}

}

h1{margin:0 0 24px;font-size:28px;font-weight:600}

input{

  width:100%;padding:14px 16px;border-radius:10px;border:1px solid #333;

  background:#050505;color:#fff;font-size:18px;text-align:center;outline:none

}

input:focus{border-color:#5b0909}

button{

  margin-top:16px;padding:13px 28px;border:1px solid #4a0909;border-radius:10px;

  background:#240404;color:#fff;font-size:17px;cursor:pointer

}
