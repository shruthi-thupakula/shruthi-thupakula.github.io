### AngularJS

- Angular is a Javascript framework that is used for building web, desktop, and mobile applications.
- Development of Angular applications involves usage of Typescript, which is a superset of Javascript, along with HTML, CSS etc.
- AngularJS extends HTML attributes with Directives(ng-directives).
- AngularJS expressions can be written inside double braces `{{ expression }}`
- AngularJS expressions can also be written inside a directive:
  `ng-bind="expression"`
- AngularJS numbers are like JavaScript numbers:

```javascript
ng - init = "quantity=1;cost=5";
```

AngularJS strings are like JavaScript strings:

```javascript
ng - init = "firstName='John';lastName='Doe'";
```

AngularJS objects are like JavaScript objects:

```javascript
ng - init = "person={firstName:'John',lastName:'Doe'}";
```

AngularJS arrays are like JavaScript arrays:

```javascript
ng - init = "points=[1,15,19,2,40]";
```

- The `ng-init` directive initializes application data.Where _ng-_ means angular.

#### Modules & Controllers:

- AngularJS **modules** define AngularJS applications.
- The module is a container for the application controllers.
- Controllers always belong to a module(**controllers** control AngularJS applications).

#### Directive:

- Directives are used to manipulate the DOM. By using Angular directives, you can change the appearance, behavior or a layout of a DOM element. It also helps you to extend HTML.

##### ng-model Directive

- With ng-model directive you can bind the value of an input field to a variable created in AngularJS.
- ng-model directive can provide type validation for application data (number, e-mail, required).
- ng-model directive can provide status for application data (valid, dirty, touched, error).
- ng-model directive provides a two-way binding between the model and the view
- two-way binding:synchronization between the model and the view

#### Scope

- The scope is the binding part between the View (HTML) and the Controller (JavaScript).
- It transfers data from the controller to view and vice-versa.

## MVC:

MVC architecture with AngularJS makes it easier to build client-side web applications. All the necessary elements are developed separately and combined automatically, which saves additional time and effort.

**Model:** AngularJS applications usually have a data model. The data model is a collection of data available for the application.

**View:** Where the AngularJS application is displayed, is called the view.

- The view has access to the model, and there are several ways of displaying model data in the view.
- You can use the ng-bind directive, which will bind the innerHTML of the element to the specified model property.

**Controller:** Applications in AngularJS are controlled by controllers.

- Because of the immediate synchronization of the model and the view, the controller can be completely separated from the view, and simply concentrate on the model data.
- To the data binding in AngularJS, the view will reflect any changes made in the controller.
- `ng-controller` directive defines the application controller.
- A controller is a JavaScript Object, created by a standard JavaScript object constructor.

#### AngularJS Data Binding

- Data binding in AngularJS is the synchronization between the model and the view.
- **Data binding:** When data in the model changes, the view reflects the change, and when data in the view changes, the model is updated as well. This happens immediately and automatically.

#### Incremental DOM (IDOM)

- It is same as Virtual DOM(VDOM-which is used in ReactJS), but with a different approach.Unlike building a representation of the DOM tree in memory(which is done by VDOM), it just uses the real DOM to diff against new trees.
- Every component gets compiled into a series of instructions. Those instructions create DOM trees and update them in-place when the data changes.

**AngularJS is perfect for database CRUD (Create Read Update Delete) applications.**

#### AngularJS vs JS:

- AngularJS expressions do not support conditionals, loops, and exceptions, while JavaScript expressions do.
- AngularJS expressions support filters, while JavaScript expressions do not.

#### AngularJS vs ReactJS:

- React is a library while Angular is a framework.
- ReactJS is easy to understand and execute while AngularJS is difficult due to third-party syntax and libraries.
- ReactJS is on Open Source Library while AngularJS is on MVC framework.
- ReactJS works on Virtual DOM while AngularJS works on Regular DOM.
- The key difference lies in it's state management. AngularJS has data binding, whereas React is generally augmented by Redux to give unidirectional data flow and work with immutable data.
- React offers better rendering performance than Angular because of its virtual DOM.
- Angular is based on Typescript and React is based on Javascript.
