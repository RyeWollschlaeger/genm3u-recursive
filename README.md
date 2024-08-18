This script is a simple Bash tool designed to generate `.m3u` playlists from audio or video files in the current directory. It scans for files with specified extensions and creates a playlist file with the name you provide. 

## Usage

```bash
./script_name <command> <playlist_name>
```

### Commands:

- `-a` or `--audio`: Creates a playlist containing all audio files (`.mp3`, `.flac`, `.aac`, `.ogg`) in the current directory.
- `-v` or `--video`: Creates a playlist containing all video files (`.mp4`, `.mkv`, `.avi`) in the current directory.
- `-h` or `--help`: Displays usage information.

### Example:

```bash
./script_name -a my_playlist
```

This command will create a playlist named `my_playlist.m3u` containing all audio files in the current directory.

