<img alt="gpt-oss-safeguard" src="./docs/gpt-oss-safeguard.png">
<p align="center">
  <strong>Download <a href="https://huggingface.co/openai/gpt-oss-safeguard-120b">gpt-oss-safeguard-120b</a> and <a href="https://huggingface.co/openai/gpt-oss-safeguard-20b">gpt-oss-safeguard-20b</a> on Hugging Face</strong>
</p>
<p align="center">
<a href="https://huggingface.co/spaces/openai/gpt-oss-safeguard-20b"><strong>Try gpt-oss-safeguard</strong></a> ·
  <a href="https://cookbook.openai.com/articles/gpt-oss-safeguard-guide"><strong>Guide</strong></a> ·
  <a href="https://arxiv.org/abs/2508.10925"><strong>Model card</strong></a> ·
  <a href="https://openai.com/index/introducing-gpt-oss-safeguard/"><strong>OpenAI blog</strong></a> 
</p>

<br>

`gpt-oss-safeguard-120b` and `gpt-oss-safeguard-20b` are safety reasoning models built-upon [gpt-oss](https://github.com/openai/gpt-oss).
With these models, you can classify text content based on safety policies that you provide and perform a suite of foundational safety tasks. These models are intended for safety use cases. For other applications, we recommend using [gpt oss models](https://huggingface.co/collections/openai/gpt-oss))

- `gpt-oss-safeguard-120b` — for production, general purpose, high reasoning use cases that fit into a single 80GB GPU (like NVIDIA H100 or AMD MI300X) (117B parameters with 5.1B active parameters)
- `gpt-oss-safeguard-20b` — for lower latency, and local or specialized use cases (21B parameters with 3.6B active parameters)

Both models were trained using our [harmony response format][harmony] and should only be used with this format; otherwise, they will not work correctly.

## Highlights

- **Trained to reason about safety:** Build freely without copyleft restrictions or patent risk—ideal for experimentation, customization, and commercial deployment.
- **Bring your own policy:** Easily adjust the reasoning effort (low, medium, high) based on your specific use case and latency needs.
- **Reasoned decisions, not just scores:** Provides complete access to the model's reasoning process, facilitating easier debugging and greater trust in outputs. This information is not intended to be shown to end users.
- **Configurable reasoning effort:** Easily adjust the reasoning effort (low, medium, high) based on your specific use case and latency needs.
- **Permissive Apache 2.0 license:** Build freely without copyleft restrictions or patent risk—ideal for experimentation, customization, and commercial deployment.

## Inference examples

You can use gpt-oss-safeguard-120b and gpt-oss-safeguard-20b similar to gpt-oss-120b and gpt-oss-20b as described in our respective [cookbooks](https://cookbook.openai.com/topic/gpt-oss).

## Policy examples

We’ve also provided a [detailed prompting guide](https://cookbook.openai.com/articles/gpt-oss-safeguard-guide), along with a [sample policy](/example_policies/spam/policy.txt) and [golden set](/example_policies/spam/golden_dataset.csv) to provide guidelines for how to craft your policy and use it with the models.

## Download the model

You can download the model weights from the [Hugging Face Hub](https://huggingface.co/collections/openai/gpt-oss-safeguard) using similar instructions to `gpt-oss-120b`.

## Join the ROOST Model Community

gpt-oss-safeguard is a model partner of the [Robust Open Online Safety Tools (ROOST) Model Community](https://roost.tools/). The ROOST Model Community (RMC) is a group of safety practitioners exploring open source AI models to protect online spaces. As an
RMC model partner, OpenAI iscommitted to incorporating user feedback and jointly iterating on future releases in pursuit of open safety. Visit the [RMC GitHub repo](https://github.com/roostorg/open-models) to learn more about this partnership and how to get involved.
