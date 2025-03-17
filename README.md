# AutoDrivingSimulation

Auto Driving Car Simulation
Overview
The Auto Driving Car Simulation is a console-based program that simulates a car navigating within a bounded field. Users can add cars, set their initial positions, and input movement commands to simulate driving. The program ensures that the cars remain within the field boundaries and follows simple movement rules.
Features
•	Define a simulation field with custom width and height.
•	Add multiple cars with unique names and starting positions.
•	Accept movement commands (L = Left, R = Right, F = Forward).
•	Prevent cars from moving out of bounds.
•	Display the final positions of all cars after simulation.
Technologies Used
•	.NET 8.0 (C#)
•	XUnit (Unit Testing)
________________________________________
Getting Started
Prerequisites
Ensure you have the following installed:
•	.NET 8 SDK
Clone the Repository
git clone https://github.com/your-repo/AutoDrivingCarSimulation.git
cd AutoDrivingCarSimulation
Build the Project
dotnet build
Run the Simulation
dotnet run --project AutoDrivingSimulation
________________________________________
Usage Guide
Starting the Simulation
Upon running the program, the user will be prompted to enter the size of the simulation field.
Welcome to Auto Driving Car Simulation!
Please enter the width and height of the simulation field in x y format:
Example input:
10 20
Adding a Car
Please choose from the following options:
[1] Add a car to field
[2] Run simulation
Enter option:
Select 1 to add a car.
Please enter the name of the car:
Example input:
Tesla
Please enter initial position of car in x y Direction format:
Example input:
5 10 N
Please enter the commands for the car:
Example input:
L F F R F
Running the Simulation
Select 2 to run the simulation.
Example output:
Executing commands...
- Tesla, (4,8) E
________________________________________
Code Structure
Car Class
Handles car properties and movement logic.
•	ExecuteCommand(char command, int width, int height): Moves and turns the car while ensuring boundary limits.
Program.cs
Manages user inputs, simulation loop, and displaying final results.
________________________________________
Running Tests
The project includes unit tests using XUnit.
Run Tests
dotnet test
Test Project Dependencies
•	coverlet.collector
•	Microsoft.NET.Test.Sdk
•	xunit
•	xunit.runner.visualstudio
Test Configuration (Autodrivingcarsimulation.Test.csproj)
<ItemGroup>
    <PackageReference Include="coverlet.collector" Version="6.0.0" />
    <PackageReference Include="Microsoft.NET.Test.Sdk" Version="17.8.0" />
    <PackageReference Include="xunit" Version="2.5.3" />
    <PackageReference Include="xunit.runner.visualstudio" Version="3.0.2">
      <PrivateAssets>all</PrivateAssets>
    </PackageReference>
</ItemGroup>


