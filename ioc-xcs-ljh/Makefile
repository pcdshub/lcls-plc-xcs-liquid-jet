IOC_TOP = /reg/g/pcds/epics/ioc/common/ads-ioc/R0.2.5
IOC_INSTANCE_PATH := $(shell pwd)

# Set PRODUCTION_IOC to 1 to move from a testing to a production IOC:
PRODUCTION_IOC := 0

PROJECT_NAME := LiquidJet
PROJECT_PATH := ../LiquidJetPLC/LiquidJet.tsproj
PLC := LiquidJetPLC

PYTMC_OPTS := 
PREFIX := PLC:$(PLC)

# With two $$, as in $$(IOCNAME) below, this will be expanded in the
# environment of st.cmd:
DB_PARAMETERS := 'PREFIX=$(PREFIX):,IOCNAME=$$(IOCNAME)'

include $(IOC_TOP)/iocBoot/templates/Makefile.base
