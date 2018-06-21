ng new adal-angular6-example --routing

cd adal-angular6-example

ng add @angular/material

npm install --save @angular/cdk

npm install --save adal-angular4

ng g component Home

ng g component NotFound

ng g component Toolbar

Edit app.routing.module:


ng g module Material

import { NgModule } from '@angular/core';
import { CommonModule } from '@angular/common';
import { MatButtonModule, MatToolbarModule } from '@angular/material';

@NgModule({
  imports: [
    CommonModule,
    MatButtonModule,
    MatToolbarModule
  ],
  exports: [
    MatButtonModule,
    MatToolbarModule
  ],
  declarations: []
})
export class MaterialModule { }

import {MaterialModule} from './material/material.module';

add to imports

