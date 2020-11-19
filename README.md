# fastapi

## conda setup

## define a new env and save

	source $HOME/miniconda/bin/activate
	conda create --name fastapi python=3.8 -y
	conda activate fastapi

### install whats needed and available via conda

	conda install --name fastapi pylint autopep8 -y

### install whats needed and available via pip

    pip install fastapi uvicorn

## Save all that in an env

	conda env export > environment.yml

## remove all

	conda env list
	conda deactivate
	conda env remove -n fastapi
    conda deactivate
	conda clean -y -t

## create again from saved environment.yml

	source $HOME/miniconda/bin/activate
	conda env create -f environment.yml
	conda activate fastapi


# run

    uvicorn main:app --reload
