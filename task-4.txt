class uber {
    constructor (baseFare,CostperKilometer,CostperMinute){
      this.baseFare = baseFare;
      this.CostperKilometer = CostperKilometer;
      this.CostperMinute = CostperMinute;
      
    }
    
    get cost(){
      return (this.baseFare + (distanceinKilometer*this.CostperKilometer) + (timeinMinutes * this.CostperMinute ));
    }
    
    
  }
  
  const details = new uber (15,2,0.5);
  
  const distanceinKilometer = 30;
  const timeinMinutes = 50;
  
  console.log("your total cost is " + details.cost);