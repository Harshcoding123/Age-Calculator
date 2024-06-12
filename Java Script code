let calculate= document.querySelector("#calculate");
let input= document.querySelector("input");
let p= document.querySelector("p");
function getDaysInMonth(y,m){
    return new Date(y,m,0).getDate();
}


calculate.addEventListener("click",()=>{
    age_calculator();

})
function age_calculator(){
    let birthDate= new  Date(input.value);
    let d1= birthDate.getDate();
    let m1= birthDate.getMonth()+1;
    let y1 =birthDate.getFullYear();
    let today= new Date();
    let d2= today.getDate();
    let m2= today.getMonth()+1;
    let y2= today.getFullYear();
    let d3,m3,y3;
    y3=y2-y1;
    if(m2>=m1){
        m3= m2-m1;

    }else{
        y3--;
        m3= 12+m2-m1;
    }
    if(d2>=d1){
        d3= d2-d1;

    }else{
        m3--;
        d3= getDaysInMonth(y1,m1)+(d2-d1);
    }
    if(m3<0){
        m3=11;
        y3--;
    }
    console.log(d3,m3,y3);
    p.innerText= `You are ${y3} Years, ${m3} Months and ${d3} Days old`;

}
