##
# @description Image to use Node.js in a development container with Vite
# @author      C. M. de Picciotto <d3p1@d3p1.dev> (https://d3p1.dev/)
##
FROM d3p1/devcontainer-node:22

##
# @note Install required dependency to avoid
#       `Error: spawn xdg-open ENOENT` error
# @link https://stackoverflow.com/questions/73942710/vitest-ui-causing-error-spawn-xdg-open-enoent
##
RUN apt install -y xdg-utils
