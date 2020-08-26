>> ### Exercise 4-1 Shape
>>
>> Design a class named Triangle that extends `Shape`. The class contains the following:
>>
>> * Three double variables named *side1*, *side2* and *side3* to denote three sides of the triangle.
>> * A constructor with no arguments, creating a triangle with each side set to *1.0*.
>> * A constructor where you can specify each side.
>> * Constant accessor functions for all three data fields.
>> * A constant function named `getArea()` that returns the area of the triangle.
>> * A constant function named `getPerimeter()` that returns the perimeter of the triangle.
>>
>> Write a test program to verify all functionallity.
>> File Shape.h
>>
>> ```cpp
>>#ifndef SHAPE_H
>>#define SHAPE_H
>>
>>#include <string>
>>
>>class Shape {
>>public:
>>  Shape();
>>  Shape(const std::string& color, bool filled);
>>  std::string getColor() const;
>>  void setColor(const std::string& color);
>>  bool isFilled() const;
>>  void setFilled(bool filled);
>>  std::string toString() const;
>>
>>private:
>>  std::string color;
>>  bool filled;
>>};
>>
>>#endif
>>```
>>
>> File Shape.cpp
>>
>> ```cpp
>>#include "Shape.h"
>>using namespace std;
>>
>>Shape::Shape() : 
>>  color("white"), filled(false) {
>>}
>>
>>Shape::Shape(const std::string& color, bool filled) :
>>  color(color), filled(filled) {
>>}
>>
>>std::string Shape::getColor() const {
>>  return color;
>>}
>>
>>void Shape::setColor(const std::string& color) {
>>  this->color = color;
>>}
>>
>>bool Shape::isFilled() const {
>>  return filled;
>>}
>>
>>void Shape::setFilled(bool filled) {
>>  this->filled = filled;
>>}
>>
>>std::string Shape::toString() const {
>>  return "Shape";
>>}
>>```
>>
>{: .exercise}