# fluent-bit-build

This builds fluent bit that actually works with authenticated kafka

## Usage

Run `build` . You'll be prompted for credentials to install build dependencies.

## Configuration of fluent-bit after install

Configuration is modular.  

Put inputs in /etc/fluent-bit/inputs.d  
Put parsers in /etc/fluent-bit/parsers.d  
Put filters in /etc/fluent-bit/filters.d  
Put outputs in /etc/fluent-bit/outputs.d  
  
This allows cloud-init to layer in configs.  
  
It'll start with a single dummy event

