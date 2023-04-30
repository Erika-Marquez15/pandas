# pandas
Libreria de python usando Pandas
import pandas as pdpython3 

def testing(numberNames=1):

    name = pd.read_csv("hombres.csv")

    if numberNames >= 2:

        result_array = []

        for i in range(numberNames):
            temporal_return = name.sample()["nombre"].to_string(index=False).strip()
            result_array.append(temporal_return)
        return result_array
    else:
        result_string = name.sample()["nombre"].to_string(index=False).strip()
        return result_string
print(testing(100))

def testing(numberNames=1):

    name = pd.read_csv("mujeres.csv")

    if numberNames >= 2:

        result_array = []

        for i in range(numberNames):
            temporal_return = name.sample()["nombre"].to_string(index=False).strip()
            result_array.append(temporal_return)
        return result_array
    else:
        result_string = name.sample()["nombre"].to_string(index=False).strip()
        return result_string

print(testing(10))
