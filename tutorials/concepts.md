![Example of a Generator Window](https://raw.githubusercontent.com/Tommycore/rnd-npcs/develop/screenshots/example_generator_window.jpg)

#### Creation
The result of a generation process.

#### Recipes
A Recipe is a blueprint for Creation.

#### Category
Categories are visual dividers, used to split up a GeneratorWindow and bundle Fields together. They have no influence on the logic, and their exclusive purpose is of an optical nature. In the picture above, the two categories "ID" and "Job" are framed in red.

#### Fields
Fields are individual aspects of a Creation, such as a name, occupation or hair colour of a person. In the picture above, the field called "First name" is framed in yellow.

#### Formula
A Formula is a blueprint for a Field.

#### Formula-Pieces
Formulas can contain one or more Pieces. A Piece is an instruction to generate a part of the Field. Think of it as textual instruction to a function call, because that is basically what it is. Pieces can be resolved as parameters of other Pieces. The general form is `[f:a0:a1:a2:...:an]`. There are always surrounding parenthesis [], with an identifier (f) followed by a number of arguments (a0-an) inside.

#### Post Processing
Postprocessing happens after all Formula-Pieces have been resolved, and is always done on the whole result. Postprocessing happens in multiple steps.

#### Post Processing Step
Each step consists of a percentual chance to be executed, and a number of options from which one is randomly picked.

#### Form Action Buttons
Form Action Buttons sit at the bottom of a generator window and allow for interaction with the created content. They're framed in blue in the picture above.