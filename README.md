# AUTO-INSURANCE-ANALYSIS

# AIM:
 To Create a Linear Regression Model to predict Employee Salaries.
# ALGORITHM:
Import and examine the data
STEP1: From the Sources palette, add a Var. File node to a blank stream canvas, 
edit the node, point to employee_data.txt, and then close the Var. File dialog 
box.
STEP2: From the Output palette, add a Table node downstream from the Var. 
File node, run it, and then examine the output. The dataset is comprised of 474 
employees.Close the Table output window.
STEP 3: From the Output palette, add a Data Audit node downstream from 
the Var. File node, run it, and then examine the output.
             
   # Set measurement levels and roles:


STEP 1: From Field Ops, add a Type node downstream from the Var. File node.
STEP 2: Edit the Type node. Click Read Values
STEP 3: set the Measurement for educational_level to Ordinal
STEP 4: The Role from gender to months_previous_experience is set to Input
STEP 5: set the Role for current_salary to Target

   # Create Linear Regression Model:


STEP 1: From the Modeling palette, add a Linear node downstream from 
the Type node.
STEP 2: Edit the Linear node. Click the Build Options tab
STEP 3: click the Basics item and clear the Automatically prepare data check box
STEP 4: click the Model Selection item and set the Model Selection method 
to Include all predictors
STEP 5: click Run
STEP 6: Edit the generated model nugget, and then click the Model Summary item in 
the pane on the left.
STEP 7: Click the Predictor Importance item in the pane on the left.
STEP 8: The job_category field is by far the most important predictor. Gender is the 
second most important field. Region and age are least important.
STEP 9: Click the Predicted by Observed item in the pane on the left.
STEP 10: The points are not scattered around the diagonal and the predicted values 
seem to break up in two categories.
STEP 11: Click the Coefficients by Observed item in the pane on the left, and then, 
from the Style list, select Table
