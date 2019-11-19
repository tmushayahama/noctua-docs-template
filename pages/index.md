---
layout: page
title: Noctua Form Documentation
permalink: /
---

# Noctua Documentation

## How the documentation is organized

Noctua Form has a lot of documentation. A high-level overview of how it’s
organized will help you know where to look for certain things:

Noctua Form Tutorials take you by the hand through a series of steps to create a
model, edit existing models and add more annotations to models. Start here if
you’re new to Noctua or GO CAMs in general. Also look at the “First steps”
below.

Topic guides discuss key topics and concepts at a fairly high level and provide
useful background information and explanation.

How-to guides are recipes. They guide you through the steps involved in
addressing key problems and use-cases. They are more advanced than tutorials and
assume some knowledge of how Noctua and Noctua Form works.

## What can you do with Noctua Form?

- Creating GO annotations
    - Creating a basic Activity Unit (MF, part of BP, occurs in CC
    - Creating a Biological Process (BP) only annotation
    - Creating a Cellular Component (CC) only annotation
    - Adding contextual information to an annotation
- Add annotations to an existing model
- View existing annotations in a model
- Choosing the right causal relation between activities (MFs)
- Adding a NOT qualifier to an annotation

With Activity Creator Form, you can create, add and view activities right in
your web browser—no special software is required.

## First steps

Are you new to Noctua and Noctua Form? This is the place to start!

From scratch: Overview | Installation
Tutorials: 


For a Quick Tutorial, check out [Quick Tutorial Docs](docs/quick-outline-tutorial.md)

For release notes, check out [Changelog](docs/changelog.md)

## Accessing the Noctua Curation Form

For workshop purposes, we’ll use noctua-dev:

<http://noctua-dev.berkeleybop.org/>

For reporting any issues: <https://github.com/geneontology/noctua-form/issues>

## Login

Before beginning new annotation or work on an existing model, you need to login.

Noctua login uses a curator’s github handle for authentication.

## Creating Go Annotations In Noctua

### Creating a basic Activity Unit (MF, part of BP, occurs in CC)

In this hands-on tutorial, you will learn how to create a basic activity using
**C. elegans** as an example:

1.  Click on ‘Create Activity’
2.  Add a Gene Product
    2.1  Type in gene name: **mpk-1** (explain that returned entities are what is
        in gpi file and therefore in NEO)
    2.2.  Autocomplete options are presented in a pop-up window
    1.  Gene products link out to respective gene product pages via dbxrefs.yaml

![](assets/img/create-autocomplete.gif)

3.  Add an MF
    1.  Search for ‘**protein kinase activity**’
    2.  Autocomplete options are presented in a pop-up window
    3.  Terms link out to AmiGO


![](assets/img/create-autocomplete-mf-linkouts.gif)


4.  Evidence code autocomplete using ECO term names
    1.  Search for ‘**direct assay**’
    2.  GO codes are indicated with bold three-letter GO code


![](assets/img/create-autocomplete-evidence.gif)


5.  Add a reference. Two options:
    1.  Cut and paste a DB and id, e.g. **PMID:31296532 OR**
    2.  Click on the +/lines symbol
        1.  Pop-up appears with a select drop-down of dbs for references: PMID,
            DOI, GO_REF
        2.  Select **PMID**
        3.  Add identifier: **31296532**


![](assets/img/create-autocomplete-ref.gif)


>   (Note that at this point you can save just your MF annotation by clicking on
>   the SAVE button. This will save the MF annotation and automatically save the
>   resulting model. However, if you want to add contextual information, such as
>   MF inputs, or a Biological Process or Cellular Component annotation, you
>   should wait until you’ve added all information before saving.)





For features, getting started with development, see the {% include doc.html name="Getting Started" path="getting-started" %} page. Would you like to request a feature or contribute?
[Open an issue]({{ site.repo }}/issues)
