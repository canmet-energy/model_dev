# NECB Primary School Energy Model Envelope Study. 

## Objective 
- Create a openstudio energy model using the FullServiceRestaurant Archetype. 
- Use the openstudio-standards library to create an NECB 2017 Primary school model. 
- Use the openstudio-standards gem to build this model using ruby. 
- Once the model is created and runs correctly. Modify the code to vary the wall conductances to 0.100, 0.180, 0.200.
- Run each simulation in its own folder including sizing runs.
- Run all the simulations in parallel to save time. 
- Use OpenStudio Standards methodology to generate the NECB model.  For example

```ruby
    require 'openstudio-standards'
    building_type = 'FullServiceRestaurant'
    template = 'NECB2017'
    epw_path = 'CAN_ON_Ottawa.Intl.AP.716280_CWEC2020.epw'
    primary_heating_fuel = "NaturalGas"
    standard = Standard.build(template)
    sizing_run_dir = File.dirname(__FILE__)
    standard.model_create_prototype_model(
      template: template,
      building_type: building_type,
      epw_file: epw_path,
      sizing_run_dir: sizing_run_dir,
      primary_heating_fuel: primary_heating_fuel,
      debug: true
    )
```

