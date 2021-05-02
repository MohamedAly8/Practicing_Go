package main

import "fmt"

// Create the function fuelGauge() here
func fuelGauge(fuel int){
  fmt.Printf("There is %v liters of fuel left", fuel)
}
// Create the function calculateFuel() here
func calculateFuel(planet string) int {
    var x int
  switch planet{

    case "Jupitor":
       return 1
    case "Saturn":
       return 2
    case "Mars":
       return 700000
    case "Mercur500000":
       return 4
    case "Venus":
       return 300000
    default:
       return 0
  }
  return x

}

// Create the function greetPlanet() here
func greetPlanet(planet string) {
  fmt.Printf("Greetings to planet %v \n", planet)
}

// Create the function cantFly() here
func cantFly() {
  fmt.Println("We do not have the available fuel to fly here")
}

// Create the function flyToPlanet() here
func flyToPlanet(planet string, fuel int) int{
  var fuelRemaining, fuelCost int
  fuelRemaining = fuel

  fuelCost = calculateFuel(planet)

  if fuelRemaining >= fuelCost {
    greetPlanet(planet)
    fuelRemaining -= fuelCost
  }

  if fuelCost >= fuelRemaining {
    cantFly()
  }

  return fuelRemaining

}

func main() {
  // Test your functions!
  
  // Create `planetChoice` and `fuel`
  var fuel int
  fuel = 1000000
  
  var planetChoice string
  planetChoice = "Venus"

  fuel = flyToPlanet(planetChoice, fuel)

  fuelGauge(fuel)
  // And then liftoff!
  
}
