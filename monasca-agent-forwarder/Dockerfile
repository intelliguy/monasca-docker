FROM monasca/agent-base:master-20170706-222054

ARG AGENT_USER="mon-agent"

# To force a rebuild, pass --build-arg REBUILD="$(DATE)" when running
# `docker build`
ARG REBUILD=1

COPY start.sh /

USER $AGENT_USER

CMD ["/start.sh", "%AGENT_USER"]
