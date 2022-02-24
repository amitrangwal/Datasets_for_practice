# Datasets_for_practice

# Use The Code Below in .ipynb or .py file to load the dataset

import pandas as pd
# https://query.data.world/s/puacihp6b6ynaib6o4cqkjhndx6hdq
#df = pd.read_csv('https://query.data.world/s/puacihp6b6ynaib6o4cqkjhndx6hdq')
url = 'https://raw.githubusercontent.com/datasciencedojo/datasets/master/titanic.csv'
r = requests.get(url, allow_redirects=True)
open('titanic.csv', 'wb').write(r.content)
titanic=pd.read_csv('titanic.csv')
