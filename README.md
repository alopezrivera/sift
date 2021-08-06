# [DARE Stratos IV](https://dare.tudelft.nl/stratos4/) Retrieval Nosecone Drift Simulation
`Antonio Lopez Rivera, 2021`

### [OpenDrift](https://opendrift.github.io/index.html) install

    cd src
    cd opendrift
    conda config --add channels conda-forge
    conda env create -f environment.yml
    conda activate opendrift
    pip install -e .

### Parameters
Open `src/__main__` to edit
- Last known nosecone coordinate from radar.
- Radar nosecone positioning uncertainty (implementation: 2 sigma radius).
- Retrieval ship coordinates.
- Retrieval ship cruise speed.
- Log output.

### Running
    conda activate opendrift
    cd src
    python3 -m drift
  
### Output

    SHIP     :: Distance to LKNRC    :: [Km]
    31.10
    SHIP     :: Travel time to LKNRC :: [min]
    67.17

    NOSECONE :: LONGITUDE forecast   :: [deg]
    -7
    0'
    25.74''

    NOSECONE :: LATITUDE forecast    :: [deg]
    36
    27'
    17.74''
  
[Back to top](#dare-stratos-iv-retrieval-nosecone-drift-simulation)
