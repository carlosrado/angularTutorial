GET STARTED
ANGULAR CLIENT (INCLUIDES TYPESCRIPT)

https://angular.io/cli for installation (easy)

ng new projectName //Creates a new project
ng serve (on project folder) //executes the server and returns the localhost

ANGULAR TUTORIAL https://www.youtube.com/watch?v=16rQyEQtpyQ&list=PLC3y8-rFHvwhBRAgFinJR8KHIrCdTkZcZ

[property]= something // bind property, class, etc.
(click) = onClick() // on click event
<input #myInput> // creates a variable myInput
<input [(ngModel)]="valueInput"> //binds the value of HTML controls (input, select, text-area) to application data
// if then or else
    <div *ngIf="displayName; then thenBlock; else elseBlock">
      
    </div>
    <ng-template #thenBlock>
      <h2>
        {{name}}
      </h2>  
    </ng-template>
    <ng-template #elseBlock>
      <h2>
        Hidden
      </h2>  
    </ng-template>
//switch
    <div [ngSwitch]="color">
      <div *ngSwitchCase="'red'">Red<div>
      <div *ngSwitchCase="'green'">Green<div>
      <div *ngSwitchCase="'blue'">Blue<div>
      <div *ngSwitchDefault>None<div>
    </div>
//for
    <div *ngFor="let color of colors; index as i">  //also you can get booleans with first,last, odd, even
      <h2>{{i}} {{color}}</h2>
    </div>

//commando for generate component (html,   css and ts files)
ng generate component componentNam
//pipes
<h2>{{person.firstName | json}}</h2>
<h2>{{5.678 | number:'1.2-3'}}</h2>
<h2>{{5.678 | number:'3.4-5'}}</h2>
<h2>{{5.678 | currency:'GBP'}}</h2>
<h2>{{5.678 | currency:'EUR'}}</h2>
<h2>{{0.4567 | percent}}</h2>
<h2>{{date |date:'short'}}</h2>
<h2>{{date |date:'shortDate'}}</h2>
//angular material (material design package)
ng add @angular/material
//new service
ng g s servicename
//add services
app.modules.ts
providers:[servicename]
//add new module
ng g m modulename

