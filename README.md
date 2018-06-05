Harkat vko 46:
Transition-harkka


HTML:
<input class="nappula" type="button" value="Painike 1" />
<input class="nappi" type="button" value="Painike 2" />
<input class="painike" type="button" value="Painike 3" />

CSS:
body {
  height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
}

.nappula {
  padding: 20px 40px;
  margin: 20px;
  font-size: 24px;
  text-align: center;
  color: white;
  background-color: #4388FF;
  border: none;
  border-radius: 15px;
  cursor: pointer;
}
.nappula:hover {
  background-color: #43e6ff; 
}
.nappula:active {
  background-color: #5c43ff;
  transition: background-color 2s;
}

.nappi {
   padding: 20px 40px;
  margin: 20px;
  font-size: 24px;
  text-align: center;
  color: white;
  background-color: red;
  border: none;
  border-radius: 15px;
  cursor: pointer;
}

.nappi:hover {
  width: 200px;
  height: 100px;
  transition: width 1s, height 3s;
}

.nappi:active {
  background-color: #ff4000;
  height: 150px;
  transition: width 1s, height 3s ease-in-out;
}

.painike {
   padding: 20px 40px;
  margin: 20px;
  font-size: 24px;
  text-align: center;
  color: white;
  background-color: green;
  border: none;
  border-radius: 15px;
  cursor: pointer;
}
 .painike:hover {
  width: 200px;
  height: 100px;
  transition: padding 0.8s linear;
}

.painike:active {
  background-color: #80ff00;
  width: 500px;
  transition: width 5s ease;
}
