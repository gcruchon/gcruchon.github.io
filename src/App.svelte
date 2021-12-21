<script>
  import { Alert, Col, Container, Row } from "sveltestrap";
  import Badge from "./Badge.svelte";
</script>

<Container>
  <h1 class="display-4">Gilles CRUCHON</h1>
  <h2 class="text-secondary mb-5">Cloud training / cert path</h2>
  <Row>
    <Col class="text-center">
      <Alert color="primary"><h3>Azure</h3></Alert>
    </Col>
    <Col class="text-center">
      <Alert color="success"><h3>Google Cloud Platform</h3></Alert>
    </Col>
  </Row>
  <Row class="cert">
    <Col>
      <Container>
        <Row>
          <Col>
            <Badge
              name="azure-fundamentals"
              certName="AZ-900"
              url="https://www.credly.com/badges/498e248a-0ca6-4bdb-ac9c-4071da44c86a/public_url"
            />
          </Col>
          <Col>
            <Badge name="azure-data-engineer-associate" certName="DP-203" />
          </Col>
          <Col>
            <Badge name="azure-ai-engineer-associate" certName="AI-102" />
          </Col>
        </Row>
      </Container>
    </Col>
    <Col>
      <Container>
        <Row>
          <Col>
            <Badge
              name="gcp-cloud-engineer-associate"
              certName="ASL Advanced Machine Learning Ops with TFX"
              url="#"
            />
          </Col>
        </Row>
      </Container>
    </Col>
  </Row>
  <Row>
    <Col class="text-center">
      <Alert color="warning"><h3>Amazon Web Services</h3></Alert>
    </Col>
    <Col class="text-center"
      ><Alert color="danger"><h3>Red Hat OpenShift</h3></Alert></Col
    >
  </Row>
  <Row class="cert">
    <Col>
      <Container>
        <Row>
          <Col>
            <Badge
              name="aws-certified-cloud-practitioner"
              certName="AWS Certified Cloud Practitioner"
            />
          </Col>
          <Col>
            <Badge
              name="aws-certified-machine-learning-specialty"
              certName="AWS Certified Machine Learning – Specialty"
            />
          </Col>
          <Col>
            <Badge
              name="aws-certified-data-analytics-specialty"
              certName="AWS Certified Data Analytics - Specialty"
            />
          </Col>
        </Row>
      </Container>
    </Col>
    <Col>
      <Container>
        <Row>
          <Col>
            <Badge
              name="redhat-openshift"
              certName="DO-180 - Containers & Kubernetes"
              url="#"
            />
          </Col>
        </Row>
      </Container>
    </Col>
  </Row>
</Container>

<style>
  h3 {
    font-size: 1.5em;
    margin: 0;
    padding: 0;
  }

  :global(.cert) {
    margin: 0.2em 0 1em 0;
  }

  :global(.cert .col) {
    margin: 0.7em;
    text-align: center;
  }

  :global(.cert .col img) {
    max-width: 150px;
  }
</style>
