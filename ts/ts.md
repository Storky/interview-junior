# TypeScript

## 1. Generic

GENERIC – is function, where types can be explicitly set as additional block of variables.

## 2. Types

Basic types
Boolean, Number, String, Array,
Tuple - let x: [string, number]; 
Enum - enum Color { Red = 1, Green, Blue, }; let c: Color = Color.Green; 
Unknown, Any, Void, Null, Undefined, Never, Object

Structural typing - let o = { x: "hi", extra: 1 } 
Unions - arg: string | string[] | (() => string) | { s: string } 
Unit types - direction: "left" | "right" 
Type Aliases - type Size = [number, number]; let x: Size = [101.1, 999.9]; 
Discriminated Unions - type Shape = | { kind: "square"; x: number } | { kind: "square"}
Type Parameters - function liftArray<T>(t: T): Array<T> { return [t]; } 


## 3. Utility types (Record)

#### Utility types

Record<Keys,Type>

type of obj, where keys from Unit type Keys, and values by Type


**Decorator** - special kind of declaration that can be attached to a class declaration, method, accessor, property, or parameter. Decorators use the form @expression, where expression must evaluate to a function that will be called at runtime with information about the decorated declaration. 
