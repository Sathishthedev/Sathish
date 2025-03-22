import { Button } from "@/components/ui/button"
import { Card, CardContent, CardDescription, CardHeader, CardTitle } from "@/components/ui/card"
import {
  DropdownMenu,
  DropdownMenuCheckboxItem,
  DropdownMenuContent,
  DropdownMenuItem,
  DropdownMenuLabel,
  DropdownMenuSeparator,
  DropdownMenuTrigger,
} from "@/components/ui/dropdown-menu"
import { Separator } from "@/components/ui/separator"
import { ChevronDown, CircleDot, GitFork, Plus, Star } from "lucide-react"

export default function GitHubCard() {
  return (
    <Card className="w-full max-w-lg">
      <CardHeader className="grid grid-cols-[1fr_110px] items-start gap-4 space-y-0">
        <div className="space-y-1">
          <CardTitle>vercel/next.js</CardTitle>
          <CardDescription>
            The React Framework for the Web. The platform for building full-stack applications.
          </CardDescription>
        </div>
        <div className="flex items-center gap-1 rounded-md bg-secondary text-secondary-foreground">
          <Button variant="secondary" className="px-3 shadow-none">
            <Star className="w-4 h-4 mr-2" />
            Star
          </Button>
          <Separator orientation="vertical" className="h-[20px]" />
          <DropdownMenu>
            <DropdownMenuTrigger asChild>
              <Button variant="secondary" className="px-2 shadow-none">
                <ChevronDown className="w-4 h-4 text-secondary-foreground" />
              </Button>
            </DropdownMenuTrigger>
            <DropdownMenuContent align="end" alignOffset={-5} className="w-[200px]" forceMount>
              <DropdownMenuLabel>Suggested Lists</DropdownMenuLabel>
              <DropdownMenuSeparator />
              <DropdownMenuCheckboxItem checked>Web Frameworks</DropdownMenuCheckboxItem>
              <DropdownMenuCheckboxItem>My Stack</DropdownMenuCheckboxItem>
              <DropdownMenuCheckboxItem>Learning Resources</DropdownMenuCheckboxItem>
              <DropdownMenuSeparator />
              <DropdownMenuItem>
                <Plus className="w-4 h-4 mr-2" /> Create List
              </DropdownMenuItem>
            </DropdownMenuContent>
          </DropdownMenu>
        </div>
      </CardHeader>
      <CardContent>
        <div className="flex flex-wrap gap-4 text-sm text-muted-foreground">
          <div className="flex items-center">
            <CircleDot className="w-3 h-3 mr-1 text-blue-500" />
            TypeScript
          </div>
          <div className="flex items-center">
            <Star className="w-3 h-3 mr-1" />
            112k
          </div>
          <div className="flex items-center">
            <GitFork className="w-3 h-3 mr-1" />
            24.5k
          </div>
          <div>Updated Feb 2025</div>
        </div>
      </CardContent>
    </Card>
  )
}

