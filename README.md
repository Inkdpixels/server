# server

> Bash function for quickly booting up a server using either flow, php or the NodeJS [http-server](https://www.npmjs.com/package/http-server) package.

## Installation
```sh
git clone https://github.com/Inkdpixels/server.git $HOME/.server-script && cd $HOME/.server-script && ./install && cd
```

## Why?
Because. No really, I am tired of executing different commands while switching between projects. I'm also lazy, and so are you! Join the Navy!

## Usage
If the server argument is executed without command line arguments, it will first check if your cwd is a valid flow application, and then boot up the flow server. If no flow application was found, it will start up the PHP server as of PHP v5.4.0, and if no PHP binary is found, it will check the `http-server` package for NodeJS.
```sh
server
```

Or, if you want to be specific and configure the command
```sh
server --type <type> --port <port>
```

## Options
| Option        | Required        | Default value  | Possible options      |
| ------------- | --------------- | -------------- | --------------------- |
| `type`        | No              | `none`         | `flow`, `php`, `node` |
| `port`        | No              | `8000`         | `INT`                 |

## License
THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
