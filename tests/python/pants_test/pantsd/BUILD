# Copyright 2020 Pants project contributors (see CONTRIBUTORS.md).
# Licensed under the Apache License, Version 2.0 (see LICENSE).

python_tests(
  sources=['test_*.py'],
  dependencies=["//:build_root"],
)

python_library(
  name = 'pantsd_integration_test_base',
  dependencies = [
    'testprojects/src/python:coordinated_runs_directory',
  ],
)

python_tests(
  name='pantsd_integration',
  sources=["pantsd_integration_test.py"],
  dependencies = [
    'testprojects/src/python:hello_directory',
    'testprojects/src/python:bad_requirements_directory',
    'testprojects/src/python:print_env_directory',
  ],
  timeout = 2100
)
