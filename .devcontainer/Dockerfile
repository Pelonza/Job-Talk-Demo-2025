# Copyright (c) UBC-DSCI Development Team.
FROM ubcdsci/py-dsci-100:20230831022048aa49aa

# Switch the working directory back to the homedir
WORKDIR ${HOME}

# Make sure the contents of our repo are in ${HOME} for binder
# Might not need these, since we aren't working in binder -- is this what changed the terminal user name?
COPY . ${HOME}
USER root
RUN chown -R ${NB_UID} ${HOME}
USER ${NB_USER}
