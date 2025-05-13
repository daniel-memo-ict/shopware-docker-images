FROM adminer

LABEL org.opencontainers.image.source https://github.com/daniel-memo-ict/shopware-docker

USER root
COPY patch.php /tmp/patch.php

RUN php /tmp/patch.php && \
	rm /tmp/patch.php

USER adminer
