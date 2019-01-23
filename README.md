	var prNum;
	prNum = Math.floor((Math.random() * 13 )+1);
	console.log(prNum);
	
	/**for (i = 0; i<3; i++) {
	if (i<3) {
	}
	else { alert("You used 3 all attempts"); }

	}
	**/

function f1() {
	var myNum, out;
	myNum = document.getElementById("myNum").value;
	out = document.getElementById("out");
	myNum = parseInt(myNum);
	
	if (myNum == prNum) {
		out.innerHTML= "Win!";
	}
	else if (myNum > prNum && myNum < 14 ) {
		out.innerHTML= "too much..";
	}
	else if (!myNum || 0 === myNum.length || myNum > 13 || myNum == typeof( "undefined" ) ){
		out.innerHTML= "You must to enter a number from 1 to 13";
	}
	else {
		out.innerHTML= "too little..";
	}
}
