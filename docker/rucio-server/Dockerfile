ARG RUCIO_VERSION

FROM rucio/rucio-server:release-$RUCIO_VERSION

RUN python3 -m pip install jlab_rucio_policy_package

ADD http://pki.jlab.org/JLabCA.crt /etc/pki/ca-trust/source/anchors/
RUN update-ca-trust
