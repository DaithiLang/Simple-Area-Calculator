# Simple-Area-Calculator
#include "stdafx.h"


void main()
{
	int choice = 0;
	float Area = 0;
	float Base = 0;
	float Height = 0;
	float Side = 0;
	float Pi = 3.14;
	float Radius = 0;
	float Angle = 0;
	float TopBase = 0;
	float SmallRad = 0;
	float BigRad = 0;
	float Width = 0;

	printf("Area Calculator\n\n");



	printf("0 \t <Quit>\n");
	printf("1 \t <Triangle>\n");
	printf("2 \t <Square>\n");
	printf("3 \t <Rectangle>\n");
	printf("4 \t <Parallelogram>\n");
	printf("5 \t <Trapezium>\n");
	printf("6 \t <Circle>\n");
	printf("7 \t <Ellipse>\n");
	printf("8 \t <Sector>\n");

	printf("Enter Choice:\t");
	scanf_s("%d", &choice);
	
	while (choice > 0)
	{
		switch (choice)
		{
		case (0q0) :
			break;
		case (1) :
			printf("Enter Base Width:  ");
			scanf_s("%f", &Base);
			printf("Enter  Height:  ");
			scanf_s("%f", &Height);

			Area = (Base * Height) / 2;
			printf("Area: %f \n", Area);
			break;
		case (2) :
			printf("Enter Side Length:  ");
			scanf_s("%f", &Side);

			Area = (Side)* (Side);
			printf("Area: %f \n", Area);
			break;
		case(3) :
			printf("Enter Width Length:  ");
			scanf_s("%f", &Width);
			printf("Enter Height Length:  ");
			scanf_s("%f", &Height);

			Area = Height * Width;
			printf("Area: %f \n", Area);
			break;
		case(4) :
			printf("Enter Base Length:  ");
			scanf_s("%f", &Base);
			printf("Enter Height Length:  ");
			scanf_s("%f", &Height);

			Area = Base * Height;
			printf("Area: %f \n", Area);
			break;
		case(5) :
			printf("Enter Base Length:  ");
			scanf_s("%f", &Base);
			printf("Enter Height Length:  ");
			scanf_s("%f", &Height);
			printf("Enter Top Base Length:  ");
			scanf_s("%f", &TopBase);

			Area = (Base*TopBase) / 2 * Height;
			printf("Area: %f \n", Area);
			break;
		case(6) :
			printf("Enter Radius Length:  ");
			scanf_s("%f", &Radius);

			Area = (Radius*Radius) * Pi;
			printf("Area: %f \n", Area);
			break;
		case(7) :
			printf("Enter Large Radius Length:  ");
			scanf_s("%f", &BigRad);
			printf("Enter Small Radius Length:  ");
			scanf_s("%f", &SmallRad);

			Area = BigRad * SmallRad * Pi;
			printf("Area: %f \n", Area);
			break;
		case(8) :
			printf("Enter Angle In Radians Length:  ");
			scanf_s("%f", &Angle);
			printf("Enter Radius Length:  ");
			scanf_s("%f", &Radius);

			Area = ((Radius*Radius)*Angle) / 2;
			printf("Area: %f \n", Area);
			break;
		default :
			printf("Invalid Choice\n");
			break;
		}
		
		printf("\n0 \t <Quit>\n");
		printf("1 \t <Triangle>\n");
		printf("2 \t <Square>\n");
		printf("3 \t <Rectangle>\n");
		printf("4 \t <Parallelogram>\n");
		printf("5 \t <Trapezium>\n");
		printf("6 \t <Circle>\n");
		printf("7 \t <Ellipse>\n");
		printf("8 \t <Sector>\n");

		printf("Enter Choice:\t");
		scanf_s("%d", &choice);
	}
   
}
