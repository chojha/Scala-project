# Scala-project
Scala project with TDD for Bill and Service charges in restaurants

object StandardBill{
  def main(args : Array[String]){
      var cola_Price : Double = 0.50
      var coffee_Price : Double = 1.00
      var cheese_Sandwitch_Price : Double = 2.00
      var steak_Sandwitch_Price : Double = 4.50
      
      calculateBill(cola_Price)
      calculateBill(coffee_Price)
      calculateBill(cheese_Sandwitch_Price)
      calculateBill(steak_Sandwitch_Price)
      calculateBill(cola_Price + coffee_Price)
      calculateBill(cola_Price + cheese_Sandwitch_Price)
      calculateBill(cola_Price + steak_Sandwitch_Price)
      calculateBill(coffee_Price + cheese_Sandwitch_Price )
      calculateBill(coffee_Price + steak_Sandwitch_Price)
      calculateBill(cheese_Sandwitch_Price + steak_Sandwitch_Price)
  }
  
  def calculateBill(x : Double) : String = x match {
      case 0.50 => println("Total Bill = cola_Price =" + 0.50)
      case 1.00 => println("Total Bill = coffee_Price =" + 1.00)
      case 2.00 => println("Total Bill = cheese_Sandwitch_Price =" + 2.00)
      case 4.50 => println("Total Bill = steak_Sandwitch_Price =" + 4.50)
      case 1.50 => println("Total Bill = cola_Price + coffee_Price =" + 1.50)
      case 2.50 => println("Total Bill = cola_Price + cheese_Sandwitch_Price =" + 2.50)
      case 5.00 => println("Total Bill = cola_Price + steak_Sandwitch_Price =" + 5.00)
      case 3.00 => println("Total Bill = coffee_Price + cheese_Sandwitch_Price =" + 3.00)
      case 5.50 => println("Total Bill = coffee_Price + steak_Sandwitch_Price =" + 5.50)
      case 5.50 => println("Total Bill = coffee_Price + steak_Sandwitch_Price =" + 5.50)
      case 6.50 => println("Total Bill = cheese_Sandwitch_Price + steak_Sandwitch_Price =" + 6.50)
  }         
}  
  
