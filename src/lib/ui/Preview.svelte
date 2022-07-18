<script>
  import Button from "./Button.svelte";
  import Card from "./Card.svelte";
  import Heading from "./Heading.svelte";
  import Section from "./Section.svelte";
</script>

<Section scheme="dark">
  <Heading size="lg">UI Preview</Heading>
  <p>Bare en dum side for å vise elementer og farger</p>
</Section>

<Section>
  <Heading size="lg">This is a light section</Heading>
  <p>Text is dark in light sections</p>

  <Card variant="dark">
    <Heading size="lg">This is a dark card</Heading>
    <Heading size="md">Medium heading</Heading>
    <Heading size="sm">Small heading</Heading>
  </Card>

  <Card variant="accent">
    <Heading size="md">Accent card</Heading>
    <Button variant="light">A button</Button>
    <Button variant="secondary">Nadeshiko</Button>
  </Card>

  <Card variant="sky">
    <Heading size="md">Fancy sunrise sky card</Heading>
    <Button variant="light" outline>Rise and shine!</Button>
  </Card>

  <Heading size="sm">Knapper</Heading>

  <Button variant="dark">Dark</Button>
  <Button variant="primary">Primary</Button>
  <Button variant="secondary">Secondary</Button>
  <Button variant="success">Success</Button>
  <Button variant="warning">Warning</Button>
  <Button variant="danger">Danger</Button>

  <Heading>Outline-knapper</Heading>
  <Button variant="dark" outline>Dark</Button>
  <Button variant="primary" outline>Primary</Button>
  <Button variant="secondary" outline>Secondary</Button>
  <Button variant="success" outline>Success</Button>
  <Button variant="warning" outline>Warning</Button>
  <Button variant="danger" outline>Danger</Button>
</Section>

<Section scheme="dark">
  <Heading size="lg">This is a dark section</Heading>
  <p>Text is bright in dark sections</p>
  <Card variant="light">
    <Heading size="lg">This is a light card</Heading>
    <Heading size="md">Medium heading</Heading>
    <Heading size="sm">Small heading</Heading>
  </Card>

  <Heading size="sm">Knapper på mørk bakgrunn</Heading>
  <Button variant="light">Light</Button>
  <Button variant="primary">Primary</Button>
  <Button variant="secondary">Secondary</Button>
  <Button variant="success">Success</Button>
  <Button variant="warning">Warning</Button>
  <Button variant="danger">Danger</Button>

  <Heading>Outline-knapper</Heading>
  <Button variant="light" outline>Light</Button>
  <Button variant="primary" outline>Primary</Button>
  <Button variant="secondary" outline>Secondary</Button>
  <Button variant="success" outline>Success</Button>
  <Button variant="warning" outline>Warning</Button>
  <Button variant="danger" outline>Danger</Button>
</Section>
