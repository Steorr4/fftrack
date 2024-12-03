# FFTrack

## Description
FFTrack is a Python-based music recognition tool that allows users to identify songs from audio input. It uses Fast Fourier Transform (FFT) for audio processing.

## Features
- Audio processing with Fast Fourier Transform (FFT)
- Command line interface for easy usage
- Song recognition from audio recording
- Song recognition from audio files
- Simple database for storing song information

## Installation
To install FFTrack, follow the steps in [INSTALLATION.md](INSTALLATION.md).

Verify the installation by running the following command:
```
fftrack --help
```

## Usage
### Database Setup
To create the database, run the following command in your terminal:
```
fftrack populate-database
```


To record audio and identify the song, run the following command in your terminal:
```
fftrack listen
```

To identify the song from an audio file, run the following command in your terminal:
```
fftrack identify <path_to_audio_file>
```


## Configuration
To configure FFTrack, run the following command in your terminal:
```
fftrack new-config <path_to_config_file>
```

Modify the configuration file as needed.

To save the configuration, run the following command in your terminal:
```
fftrack save-config <path_to_config_file>
```

## Testing

To run the tests for this project, run the following command in your terminal:
```
coverage run -m pytest
```

To generate a coverage report, run the following command in your terminal:
```
coverage report
```

We aim for a test coverage of at least 80% for this project.

To write new tests, create a new file in the `tests` directory with the following naming convention:
```
test_<module_name>.py
```



## Contributing

If you want to contribute to this project, please follow these steps:
- Fork the repository: [FFTrack](https://github.com/schuldt-ogre/fftrack)
- Create a new branch for your feature or bug fix
- Make your changes and commit them with a meaningful message
- Push your changes to your branch
- Create a pull request against the main repository

Follow the coding standards and practices described in [DEVELOPMENT.md](DEVELOPMENT.md).



## License

This project is licensed under the GNU General Public License v3.0 - see the [LICENSE](LICENSE) file for details.
