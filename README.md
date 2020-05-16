# HowTo

## Setup you computer environment

We assume you have python installed on your computer with anaconda python distro

```
conda  create -n aci-learning-labs anaconda
conda activate aci-learning-labs
pip install acicobra-4.2_3h-py2.py3-none-any.whl
pip install acimodel-4.2_3h-py2.py3-none-any.whl
git clone https://github.com/datacenter/acitoolkit.git
cd acitoolkit
python setup.py install
```
Everything will be installed in /Users/schoen/opt/anaconda3/envs/aci-learning-labs/

```
cd ../apic_fabric_setup
python baseline.py
```

## Use sample scritps
Configure the sandbox credentials in credentials.py

```
cd acitoolkits/samples/
cat ../../sbx-intro-aci/credentials.py > credentials.py

Run any of the examples and examin the output

```
cd acitoolkit/samples
python aci-show-epgs.py
```

## Write your own scripts

## ACI Diagram
To use ACI Diagram appliacation install the graphviz on your computer
```
brew upgrade graphviz
```

Install graphviz inside of the virtual enviroment
```
pip install pygraphviz \
  --install-option="--include-path=/usr/local/include/graphviz/" \
  --install-option="--library-path=/usr/local/lib/graphviz"
```
