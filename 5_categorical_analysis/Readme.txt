"english"
---> NOMENCLATURE OF NOTEBOOKS
The analyzes are all carried out with discrete variable features (in the codes categorized according to percentiles) but
The target can vary between being a continuous variable (original value) or being a discrete variable (transformed based on
percentiles in the example codes). The nomenclature of notebooks refers to the type of variable used:
- x_cat: features are categorical/discrete variables
- y_cat: target is categorical/discrete variables
- y_cont: target is continuous variable


---> EXPLANATION
The transformation consists of categorizing the features and targets into percentiles and performing applicable analyzes for data
categorical.

The transformations to features and target are the following:
- features: categorize by percentiles and delete continuous values of variables
- target: categorize by percentiles and also maintain the continuous values of the variables

Thus, perform analysis of discrete features vs. continuous target and also of discrete features vs. discrete target.
Remember that the segmentation part is designed to categorize/segment the data based on the condition of some
variable, which can be the target, so at that stage the missing analysis of continuous feature and discrete target can be carried out

The percentiles enabled in these codes to categorize the data are:
- quartiles
- quintiles
- deciles



------------------------------------------------------------------------
"español"
---> NOMENCLATURA DE LOS NOTEBOOKS
Los análisis se realizan todos con features variables discretas (en los códigos categorizadas de acuerdo a percentiles) pero
el target puede variar entre ser una variable continua (valor original) o ser una variable discretas (transformada en base a
percentiles en los códigos de ejemplo). La nomenclatura de los notebooks hace referencia al tipo de variable que se utiliza:
	- x_cat: features son variables categóricas/discretas
	- y_cat: target es variables categóricas/discretas
	- y_cont: target es variable continua


---> EXPLICACIÓN
La transformación consiste en categorizar las features y target en percentiles y realizar análisis aplicables para datos
categóricos.

Las transformaciones a features y target son las siguientes:
- features: categorizar por percentiles y borrar los valores continuos de las variables
- target: catetegorizar por percentiles y además mantener los valores continuos de las variables

Así realizar análisis de features dicretas vs target continuo y además de features discretas vs target discreto.
Recordar que en la parte de segmentation está pensada para categorizar/segmentar los datos basado en la condición de alguna
variable, la cual puede ser el target, así en esa etapa se puede realizar el análisis faltante de feature continua y target discreto

Los percentiles habilitados en estos códigos para categorizar los datos son:
- cuartiles
- quintiles
- deciles