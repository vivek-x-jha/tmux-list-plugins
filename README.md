tmux-list-plugins
=================

Plugin that displays currently loaded plugins in `$TMUX_PLUGIN_MANAGER_PATH`.

_Note: this is the example plugin from [tpm/docs/how_to_create_plugin](https://github.com/tmux-plugins/tpm/blob/master/docs/how_to_create_plugin.md)._

Installing
----------

### Via TPM (recommended)

The easiest way to install `tmux-list-plugins` is via the [Tmux Plugin Manager](https://github.com/tmux-plugins/tpm).

1.  Add plugin to the list of TPM plugins in `.tmux.conf`:

    ``` tmux
    set -g @plugin 'vivek-x-jha/tmux-list-plugins'
    ```

2.  Use <kbd>prefix</kbd>–<kbd>I</kbd> install `tmux-list-plugins`. You should now
    be able to `tmux-list-plugins` immediately.
3.  When you want to update `tmux-list-plugins` use <kbd>prefix</kbd>–<kbd>U</kbd>.

### Manual Installation

1.  Clone the repository

    ``` sh
    $ git clone https://github.com/vivek-x-jha/tmux-list-plugins ~/clone/path
    ```

2.  Add this line to the bottom of `.tmux.conf`

    ``` tmux
    run-shell ~/clone/path/list-plugins.tmux
    ```

3.  Reload the `tmux` environment

    ``` sh
    # type this inside tmux
    $ tmux source-file ~/.tmux.conf
    ```

You should now be able to use `tmux-list-plugins` immediately.

## Usage

Use <kbd>prefix</kbd>–<kbd>T</kbd> to invoke plugin
