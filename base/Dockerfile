FROM node:8-slim
COPY qshell /usr/local/bin/qshell
COPY ossutil /usr/local/bin/ossutil
RUN npm install gitbook gitbook-cli -d -g && \
    rm /usr/local/bin/gitbook && \
    ln -s /usr/local/lib/node_modules/gitbook-cli/bin/gitbook.js /usr/local/bin/gitbook && \
    gitbook alias /usr/lib/node_modules/gitbook && \
    chmod +x /usr/local/bin/qshell && \
    chmod +x /usr/local/bin/qshell
