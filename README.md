<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Cricket Live Scores</title>

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:Arial,sans-serif;
}

body{
    background:#f5f7fb;
}

header{
    background:#00b050;
    color:white;
    padding:15px;
    text-align:center;
    font-size:24px;
    font-weight:bold;
}

.container{
    max-width:1000px;
    margin:auto;
    padding:20px;
}

.match-card{
    background:white;
    border-radius:12px;
    box-shadow:0 2px 8px rgba(0,0,0,.1);
    padding:20px;
    margin-bottom:15px;
    cursor:pointer;
    transition:.3s;
}

.match-card:hover{
    transform:translateY(-3px);
}

.live{
    color:red;
    font-weight:bold;
}

.teams{
    display:flex;
    justify-content:space-between;
    margin:15px 0;
    font-size:20px;
    font-weight:bold;
}

.score{
    font-size:22px;
    color:#00b050;
    margin-bottom:10px;
}

.details{
    display:none;
    margin-top:15px;
    border-top:1px solid #ddd;
    padding-top:15px;
}

table{
    width:100%;
    border-collapse:collapse;
}

th,td{
    border:1px solid #ddd;
    padding:8px;
    text-align:center;
}

th{
    background:#00b050;
    color:white;
}

.commentary{
    background:#f1f1f1;
    padding:10px;
    border-radius:8px;
    margin-top:15px;
}

.status{
    color:#555;
    margin-top:10px;
}

@media(max-width:600px){
    .teams{
        flex-direction:column;
        gap:10px;
    }
}
</style>
</head>

<body>

<header>
🏏 CREX Style Cricket Live Scores
</header>

<div class="container">

<div class="match-card" onclick="toggleDetails('m1')">
<div class="live">🔴 LIVE</div>

<div class="teams">
<div>INDIA</div>
<div>AUSTRALIA</div>
</div>

<div class="score">
IND 185/4 (18.2)
</div>

<div class="status">
India need 15 runs from 10 balls
</div>

<div class="details" id="m1">

<h3>Scorecard</h3>

<table>
<tr>
<th>Batsman</th>
<th>R</th>
<th>B</th>
<th>4s</th>
<th>6s</th>
</tr>

<tr>
<td>Virat Kohli</td>
<td>72</td>
<td>45</td>
<td>8</td>
<td>2</td>
</tr>

<tr>
<td>Hardik Pandya</td>
<td>35</td>
<td>18</td>
<td>3</td>
<td>2</td>
</tr>
</table>

<div class="commentary">
<h3>Ball By Ball</h3>
<p>18.2 - FOUR! Kohli drives through covers.</p>
<p>18.1 - Single taken.</p>
<p>17.6 - SIX! Hardik clears the ropes.</p>
</div>

</div>
</div>

<div class="match-card" onclick="toggleDetails('m2')">
<div class="live">🔴 LIVE</div>

<div class="teams">
<div>ENGLAND</div>
<div>PAKISTAN</div>
</div>

<div class="score">
ENG 142/6 (17.5)
</div>

<div class="status">
England batting first
</div>

<div class="details" id="m2">

<h3>Scorecard</h3>

<table>
<tr>
<th>Batsman</th>
<th>R</th>
<th>B</th>
<th>4s</th>
<th>6s</th>
</tr>

<tr>
<td>Buttler</td>
<td>55</td>
<td>34</td>
<td>5</td>
<td>3</td>
</tr>

<tr>
<td>Livingstone</td>
<td>28</td>
<td>16</td>
<td>2</td>
<td>2</td>
</tr>
</table>

<div class="commentary">
<h3>Ball By Ball</h3>
<p>17.5 - Dot ball.</p>
<p>17.4 - FOUR!</p>
<p>17.3 - WICKET!</p>
</div>

</div>
</div>

</div>

<script>

function toggleDetails(id){
    let details=document.getElementById(id);

    if(details.style.display==="block"){
        details.style.display="none";
    }else{
        details.style.display="block";
    }
}

</script>

</body>
</html><footer style="
text-align:center;
padding:15px;
background:#00b050;
color:white;
font-weight:bold;
margin-top:20px;">
Created by REBEL STAR 112
</footer>
