###  DIN UPPGIFT: Besvara följande fråga i denna md-fil / 3 poäng

 I Typescript kan både type och interfaces användas för att skapa egna sammansatta typer. I många fall kan man använda antingen type eller interfaces, men det finns också skillnader. Redogör för dem och visa med kodexempel. 

Interface kan utökas genom att andra interface kombineras med hjälp av extends.
type kan kombineras med hjälp av unions och intersectioner, men det stöder inte direkt utvidgning.

Exempel med skillnader:

//Type:

type PersonType = {
  name: string;
  age: number;
};

// Interface:

interface PersonInterface {
  name: string;
  age: number;
}

//Utvidgning med interface: 

interface Employee extends PersonInterface {
  salary: number;
}

//Type med union och intersection:

type UnionType = string | number;
type IntersectionType = { x: number } & { y: number };