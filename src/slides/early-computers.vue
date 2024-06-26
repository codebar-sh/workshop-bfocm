<template>
	<section>
		<section>
			<h3>Computers in Early Days</h3>
			<ul>
				<li class="fragment">1940 - <a href="https://en.wikipedia.org/wiki/Bombe">Bombe</a></li>
				<li class="fragment">1945 - <a href="https://en.wikipedia.org/wiki/ENIAC">ENIAC</a></li>
				<li class="fragment">1951 - <a href="https://en.wikipedia.org/wiki/UNIVAC">UNIVAC</a></li>
				<li class="fragment">1952 - <a href="https://en.wikipedia.org/wiki/IBM_701">IBM 701</a> (30 were sold in 1953-54)</li>
				<li class="fragment">1954 - <a href="https://en.wikipedia.org/wiki/IBM_650">IBM 650</a> (120 were sold in 1954, and more than 750 orders)</li>
			</ul>
		</section>
		<section>
			<h3>Users stopped building their own machines</h3>
			<h4 class="fragment">Why was IBM so late getting into computers?</h4>
		</section>
		<section>
			<h3>Programmer's view of IBM 650</h3>
			<ul>
				<li class="fragment">A machine with 44 instructions</li>
				<li class="fragment">Instruction: <code>60 1234 1009</code>
					<ul class="fragment">
						<li>Load the contents of location <code>1234</code> into the <span class="italic">distribution</span>; put it also into the <span class="italic">upper accumulator</span>; set the <span class="italic">lower accumulator</span> to zero; and then go to the location <code>1009</code> for the next instruction.</li>
					</ul>
				</li>
			</ul>
		</section>
		<section>
			<h3>Computers in mid 50's</h3>
			<ul>
				<li class="fragment">Hardware was super expensive</li>
				<li class="fragment">Stores were small (1000 words)</li>
				<li class="fragment">Programmer's view of the machine was inseparable from the actual hardware implementation</li>
			</ul>
		</section>
		<section>
			<h3>Snow White and the Seven Dwarfs (1960s)</h3>
			<ul>
				<li>IBM</li>
				<li>UNIVAC</li>
				<li>GE (General Electric)</li>
				<li>Burroughs</li>
				<li>NCR</li>
				<li>CDC (Control Data Corporation)</li>
				<li>RCA</li>
				<li>Honeywell</li>
			</ul>
		</section>
		<section>
			<h3>Compatibility Problem at IBM</h3>
			<ul>
				<li class="fragment">For engineering and scientific use: 701, 704, 709, ...</li>
				<li class="fragment">For commercial or data processing use: 702, 705, ...</li>
				<li class="fragment">Mid-range business small mainframe: 1400 series</li>
			</ul>
			<h4 class="fragment">They had completely different instruction sets, I/O system, storage, softwares, etc</h4>
		</section>
		<section>
			<h3>IBM System/360</h3>
			<ul>
				<li class="fragment">Announced on April 7, 1964. Delivered between 1965 and 1978.</li>
				<li class="fragment">Introduced a new layer of <span class="strong">abstraction</span> now well known as <span class="text-red-500">ISA</span> (instruction set architecture).</li>
				<li class="fragment">ISA specifies <span class="text-red-500 italic">what</span> hardware provides, not <span class="text-red-500 italic">how</span> it's implemented.</li>
				<li class="fragment">It was revolutionary and extraodinarily challenging, see <a href="https://en.wikipedia.org/wiki/The_Mythical_Man-Month">The Mythical Man-Month / 人月神话</a></li>
			</ul>
		</section>
		<section>
			<ProblemStack3 />
		</section>
		<section>
			<h3>Famous ISAs and Microarchitectures</h3>
			<table>
				<tr>
					<th>x86_64</th>
					<th>ARMv8</th>
				</tr>
				<tr>
					<td>
						<ul>
							<li>Intel 8086 (1978)</li>
							<li>Intel Pentium (1993)</li>
							<li>Intel Core 6th-gen Skylake (2015)</li>
							<li>AMD Zen 4 (2022)</li>
						</ul>
					</td>
					<td>
						<ul>
							<li>Apple Silicon</li>
							<li>Samsung Exynos</li>
							<li>Qualcomm Snapdragon</li>
						</ul>
					</td>
				</tr>
			</table>
			<div>PowerPC, MIPS, RISC-V, SPARC, ...</div>
		</section>
		<section>
			<h3>The Tradeoffs of ISA</h3>
			<ul>
				<li class="fragment">Enables fast innovation in hardware w/ no need to change the software</li>
				<li class="fragment">Commercially successful ISAs last for decades</li>
			</ul>
		</section>
	</section>
</template>

<script setup lang="ts">
import ProblemStack3 from "../components/problem-stack-3.vue";
</script>

<style scoped>
</style>
