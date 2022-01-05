# Continuous Previews

Source for: <https://www.cpmanifesto.org>

> Continuous Preview(s) are an automation-enabled method by which in-progress development branches—known as topic branches—are continuously deployed in a dynamic production-like environment and are available for collaborative review and testing at a secure URL. By this method iterative feedback is accelerated and testing is conducted in a logical sequence where topic branch functionality testing is completed prior to integration testing and delivery (CP, then Cl / CD).

## Structure

This repository is built using [MkDocs](https://www.mkdocs.org/), a fast and simple static site generator. Documentation source files are written in [Markdown](https://www.markdownguide.org/).

## Usage

You can build a container image that serves these documents. `docker build -t cpmanifesto .` will compile all of the Markdown into static files (HTML, CSS, etc.) and install them into an `nginx` image.  You can then serve it by running `docker run --network host cpmanifesto` and pointing your web browser to <http://localhost>.

Alternatively, you can install and run MkDocs locally on your workstation as described here: <https://www.mkdocs.org/getting-started/>

## Authorship

Primary Authors: Josh Thurman and Grayson Adkins
