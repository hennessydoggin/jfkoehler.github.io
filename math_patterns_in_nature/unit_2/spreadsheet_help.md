# Spreadsheets and Patterns

**Goals**:

- use google sheets to explore simple and compound interest problems

- create visualizations using column data in sheets

---

#### Getting Started

First, we want to start a new spreadsheet.  Click the new blank spreadsheet button to create a new blank spreadsheet.

![](https://github.com/jfkoehler/foundations/blob/master/spreadsheets/spread_I.png)

We will first create a column to act as an index.  Because we are dealing with problems about simple and compound interest, this index will usually represent the month and the value in the column will equal the balance in the account.  

We will refer to each cell as a combination of the horizontal row location and the vertical column.  The image below displays some cells with their locations named within the cells themselves.

<p align="center">
<img src="https://github.com/jfkoehler/foundations/blob/master/spreadsheets/pics/cell_local.png"
</p>

By clicking on the first cell, you are able to edit it.  We will title this cell "Month" to represent the month of the interest payment.
Further, we will start with month = 0 by typing 0 in the cell below it.  Now the good part.  Of course, we want the numbers 1, 2, 3, 4, 5, etc. to follow.  We could simply type this, but instead we can generate a pattern using an equation.  In the cell below we will type:

```
  =A1 + 1
 ```
 
This will add 1 to the first cell. Hit enter.

<p align="center">
<img src="https://github.com/jfkoehler/foundations/blob/master/spreadsheets/pics/formula_I.png"
</p>

Now, we can extend the pattern by dragging the bottom corner of the cell down.  Simply click cell `A2` in the lower right corner and drag it down to however far you would like to go.


<p align="center">
<img src="https://github.com/jfkoehler/foundations/blob/master/spreadsheets/pics/drag_I.png"
</p>

#### No Interest

Recall our problem dealing with a debt starting at $4400 and paying \$400 with no interest.  We can generate the terms of this sequence in a similar manner as to our months column.  Next to the month column, type another column heading titled "No Interest".  Our starting place  is $4400, so we will type 4400 in the second cell in the column.  Finally, we want to generate a list of terms that reflect paying the $400 each month.  Similar to last month, we will repeatedly perform an operation, however now it is subtraction by 400.  We again us the formula `= prev_cell - 400`. 

<p align="center">
<img src="https://github.com/jfkoehler/foundations/blob/master/spreadsheets/pics/formula_2.png"
</p>

<p align="center">
<img src="https://github.com/jfkoehler/foundations/blob/master/spreadsheets/pics/drag_2.png"
</p>

##### Graphing the Balance

Making a graph of the declining balance is easy.  Simply highlight the cells that contain the months and balance columns, and select the `chart` from the **insert** menu as shown below:

<p align="center">
<img src="https://github.com/jfkoehler/foundations/blob/master/spreadsheets/pics/chart_menu.png" data-canonical-src="https://github.com/jfkoehler/foundations/blob/master/spreadsheets/pics/chart_menu.png"  width="400" height="500" align="middle" />
</p>

We can choose a scatter plot to display a series of points that represent the balance at any point in time.

<p align="center">
<img src="https://github.com/jfkoehler/foundations/blob/master/spreadsheets/pics/scatter_I.png"
</p>

#### Applying Interest 

The other situation discussed involved applying an interest rate to the balance in the account at the end of each month.  Here, we apply a monthly interest rate of 1.2%.  Recall that our formula assumed that we would have interest applied after the first month to the remaining balance once a month.  

$$\text{new_balance = old_balance - 400 + interest_on_whats_left}$$

This is demonstrated with the following formula using a similar logic to the first example.

<p align="center">
<img src="https://github.com/jfkoehler/foundations/blob/master/spreadsheets/pics/formula_3.png"
</p>

Next, we may want to graph both the no interest situation and the credit card situation together.  This example uses a line graph, following the same logic as the above example as show below:

<p align="center">
<img src="https://github.com/jfkoehler/foundations/blob/master/spreadsheets/pics/graph_II.png"
</p>

#### Final Spreadsheet

In the end, you may want to customize some elements of the spreadsheet after having inserted your chart by adding some color or additional customizations.

<p align="center">
<img src="https://github.com/jfkoehler/foundations/blob/master/spreadsheets/pics/final.png"
</p>
