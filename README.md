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



Animation -harkka

HTML
<div class="switch">
  <input id="cmn-toggle-1" class="cmn-toggle cmn-toggle-round" type="checkbox">
  <label id=toggle for="cmn-toggle-1"></label>
</div>

CSS
body {
  height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
}

.cmn-toggle {
  visibility: hidden;
}
.cmn-toggle + label {
  display: block;
  position: relative;
  cursor: pointer;
}
.cmn-toggle-round + label {
  width: 500px;
  height: 60px;
  background-color: #00ff40;
  border-radius: 70px;
}
.cmn-toggle-round + label:before,
.cmn-toggle-round + label:after {
  display: block;
  position: absolute;
  top: 1px;
  left: 1px;
  bottom: 1px;
  content: "";
}
.cmn-toggle-round + label:before {
  right: 1px;
  background-color: #f1f1f1;
  border-radius: 60px;
}
.cmn-toggle-round + label:after {
  width: 58px;
  background-color: #0000ff;
  border-radius: 100%;
  box-shadow: 0 5px 5px rgba(0, 0, 0, 0.3);
}
.cmn-toggle-round:checked + label:before {
  background-color: #90B9FF;
}
.cmn-toggle-round:checked + label:after {
  @keyframes toggle {
  0% {
    margin-left: 0px;
  }
  25% {
    margin-left: 111px;
  }
  50% {
    margin-left: 223px;
  }
      75% {
    margin-left: 334px;
  }
  100% {
    margin-left: 445px;
}
 
    #toggle {
      animation: toggle 5s infinite;
    }
  }
