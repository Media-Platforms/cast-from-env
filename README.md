# cast-from-env

Get and cast environment variables

## Installation

`python setup.py install`

## Examples

    from cast_from_env import from_env

    from_env('STRING_VAR', 'default value')  # Value or 'default value' if not set
    from_env('INTEGER_VAR', 100)  # Value cast to int, or 100 if not set
    from_env('INTEGER_VAR', int)  # Value cast to int, or None if not set
    from_env('FLOAT_VAR', 1.0)  # Value cast to float, or 1.0 if not set
    from_env('TRUE_VAR', bool)  # True if value is '1', 'true', 'yes', or 'on'
    from_env('TRUE_VAR', True)  # True if value is '1', 'true', 'yes', 'on', or not set
