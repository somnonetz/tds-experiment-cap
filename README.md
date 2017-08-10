# TDS Experiment CAP

This is an experiment description for the [Time-Delay-Stability (TDS) Matlab](https://github.com/somnonetz/cc-tds-app)
application, which is compatible with [FAICE](https://github.com/curious-containers/faice) (Fair Collaboration and
Experiments) tools.

This experiment is related to somnonetz/[tds-xperiment](https://github.com/somnonetz/tds-experiment) but uses
a publicly accessible EDF file from [The CAP Sleep Database](https://physionet.org/pn6/capslpdb/#the-cap-sleep-database)
as input.


## Usage

The experiment is based on the `docker.io/curiouscontainers/cc-tds-app:cloudam2017` container image.

Install [FAICE](https://github.com/curious-containers/faice) tools, to run an experiment.


### Option 1 (Curious Containers)

Create a Vagrant VM and run the experiment locally with Curious Containers. Input and result files will be accessed in
the local file system.

```bash
faice vagrant https://raw.githubusercontent.com/somnonetz/tds-experiment-cap/master/curious-containers/tds-experiment-cap.json
```

### Option 2 (Curious Containers)

Create a Vagrant VM and run the experiment locally with Curious Containers. Input and result files will be accessed in
[XNAT](https://xnat.f4.htw-berlin.de/xnat/).

```bash
faice vagrant --remote-input-data https://raw.githubusercontent.com/somnonetz/tds-experiment-cap/master/curious-containers/tds-experiment-cap.json
```
