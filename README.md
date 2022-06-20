# pokemonpratice
Practicing coding by trying to find the best team in Pokemon Go.

Will continue to add as I continue this personal project.

At the moment, I tried to just find the effectiveness of each pokemon's type (up to Gen VI).

#### Here is how I calculated effectiveness:

For each type, I assigned values for its effectiveness against all other types. I followed this image as a guide: ![Types info](https://upload.wikimedia.org/wikipedia/commons/thumb/9/97/Pokemon_Type_Chart.svg/492px-Pokemon_Type_Chart.svg.png?20211121042045)

The blank spots are just 1, while all the other values are considered and used. The nice thing about this image is that it is pretty much a matrix with the rows representing a type attacking and columns representing a type defending.

If a pokemon has only one type, all the elements in the attacker row for that type will be summed up as well as its type's defender column. Both values for attack and defend will be divided by 18, equaling the pokemon's type effectiveness.

If a pokemon has two types, then the attacks of each type will be added together and so will the defense values. These values are divided by 36 instead of 18.

The next step now is to include base stats and compare. Specifics will be included as the project is updated.

#### Sources
Dataset: https://www.kaggle.com/datasets/rounakbanik/pokemon
Image: https://commons.wikimedia.org/wiki/File:Pokemon_Type_Chart.svg

