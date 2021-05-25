SDF should be the same with the following difference:

 * one_sdf_example_no_bug: unified world with hinged_door model embedded directly
 * include_sdf_example_bug: hinged_door model is independent. foo.world includes it via `<include>`

Reproduce bug by:

 * Installing gazebo9 (bug is not present in gazebo11):
 * `GAZEBO_MODEL_PATH=${GAZEBO_MODEL_PATH}:${PWD} gazebo --verbose foo.world`
